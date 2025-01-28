---
title: Example 04
---

import products from '../reusable-content/products.json';

:::info EXAMPLE DESCRIPTION
This example shows how a table can be generated using data found in a JSON file.
:::

## Groceries Products

<table>
  <thead>
    <tr>
      <th>Title</th>
      <th>Description</th>
      <th>Price</th>
    </tr>
  </thead>
  <tbody>
    {products.filter(product => product.category === 'groceries').map(product => (
      <tr key={product.id}>
        <td>{product.title}</td>
        <td>{product.description}</td>
        <td>${product.price}</td>
      </tr>
    ))}
  </tbody>
</table>

