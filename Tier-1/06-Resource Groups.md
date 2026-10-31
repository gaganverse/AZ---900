# Resource Groups

## Definition

A Resource Group is a **logical container for Azure resources**.

## Why?

It makes resources easier to:

- **Manage**
- **Monitor**
- **Delete**
- **Apply permissions**

## Example

```text
RG-Production
  ├── VM
  ├── Storage Account
  ├── VNet
  └── Database
```

## When to Use

Resource Groups have a common:

- **Lifecycle**
- **Application**
- **Environment**

## ⭐ Important

Deleting a resource group can delete the resources inside it.
