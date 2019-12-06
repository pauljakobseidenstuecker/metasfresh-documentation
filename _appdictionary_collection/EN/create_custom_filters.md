---
title: Create custom filters
layout: default
tags:  
  - Window
lang: en
sequence:
ref: create_custom_filters
---

## Overview
This guide shows you how to create a custom filter in a window. In general, you can use general SQL operators, such as the `LIKE` operator, but you will also need to use the field separator (`<^>`) or the segment separator (`<~>`) to write your query.

<p style="margin-left: 40px">
<strong>Example:</strong><br>
If you want to create a user query that will filter for all invoice candidates with the invoice rule "After delivery (D)", the pure SQL code using the <code>LIKE</code> operator would be: <code>InvoiceRule LIKE 'D'</code>.<br><br>
But if you write it like that, it will not work because it will not know how to parse that SQL.
So the correct way would be: <code><^>InvoiceRule<^> LIKE <^>D<^></code>.
</p>

Note the spaces before and after the `LIKE` operator. **They are essential!**

Also, note `<^>`. This is the field separator. It marks the search field, the operator and the value.<br>
For multiple terms, there is the segment separator, which looks like this: `<~>`.

<p style="margin-left: 40px">
<strong>Example:</strong><br>
If you wanted to filter for invoice candidates with the invoice rule "After delivery (D)" as well as for a certain partner, the query would look like this:<br>
<code>AND<^>InvoiceRule<^> LIKE <^>D<^><~>AND<^>Bill_BPartner_ID<^>=<^>2156423<^></code>.
</p><br>

| **Important!** |
| :--- |
| The name of the column must be the exact same one as in `AD_Column.ColumnName`. |

## Steps
Let's use a practical example. Assume you want to create a filter for the "Attribute Value" window. This filter shall include the following filtering options: *Name*, *Attribute* and *IsActive flag*.

1. Go to the window "User Query".
1. Pick the <abbr title="AD_Table_ID">table</abbr> for which you want to use the filter.
1. Pick the <abbr title="AD_Tab_ID">tab</abbr> for which you want to show the filter.
1. Enter the filtering code:<br>
   <kbd><img src="https://user-images.githubusercontent.com/15378036/70225460-c0a73a80-1757-11ea-8a64-d934ac7d89e6.PNG" alt="filter"></kbd>

1. This will result in:<br>
   <kbd><img src="https://user-images.githubusercontent.com/15378036/70226875-45935380-175a-11ea-9083-090e6b875989.png" alt="attr1"></kbd>
   <br><br>
   <kbd><img src="https://user-images.githubusercontent.com/15378036/70226881-4cba6180-175a-11ea-951d-27454d572441.png" alt="attr2"></kbd>