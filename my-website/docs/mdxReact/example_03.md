---
title: Example 03
---


import data from '../reusable-content/accessRoles.json';

:::info EXAMPLE DESCRIPTION
This example shows how to import structured content from a JSON file.
:::

## Contact data access roles

### Create contacts
The following user roles have permission to create contacts:

{data.contacts.create.map(item => (
    <div key={item}>- {item}</div>
))}

### Read contact data
The following user roles have permission to read contacts:

{data.contacts.read.map(item => (
    <div key={item}>- {item}</div>
))}

### Update contacts
The following user roles have permission to update contacts:

{data.contacts.update.map(item => (
    <div key={item}>- {item}</div>
))}

### Delete contacts
The following user roles have permission to delete contacts:

{data.contacts.delete.map(item => (
    <div key={item}>- {item}</div>
))}

