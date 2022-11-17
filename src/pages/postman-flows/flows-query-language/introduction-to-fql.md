---
title: "Introduction to FQL"
page_id: "introduction-to-fql"
updated: 2022-11-16
order: 0
warning: false
---

_Flows Query Language_ (FQL) can be used to parse and transform JSON data to get the fields and structure you want.

## Passing data to the Evaluate block

![](https://assets.postman.com/postman-labs-docs/flows-query-language/updated-evaluate-block-example.png)

The record block holds formatted key-value pairs. The variable data_field has a value of input (input can be selected as a value when creating the variable), which allows the formted data to be passed into the evaluate block and queried. In this case, customer_info holds another record that contains string values. FQL can  be executed in the evaluate block in order to print out the values of customer_info.

## Things you can do with FQL

The following sections show examples of things you can do with FQL:

- [Getting basic values](/postman-flows/flows-query-language/getting-basic-values/)
- [Conditional data selection](/postman-flows/flows-query-language/conditional-data-selection/)
- [Returning structured data](/postman-flows/flows-query-language/returning-structured-results/)
- [Data manipulation](/postman-flows/flows-query-language/data-manipulation/)