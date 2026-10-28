
# 23. RBAC (Role-Based Access Control)

## Definition

It controls access to Azure resources based on assigned roles.

## Why?

Implements **least privilege**.

## Example

```text
User
  ↓
Reader role
  ↓
Can view resources
Cannot modify them
```

## Other Common Roles

- **Owner** → Can manage resources + assign **access**
- **Contributor** → Can manage resources but cannot assign RBAC **access**
- **Reader** → Can view resources but cannot modify them

## When to Use

Use RBAC when you need to control **who can do what on Azure resources**.

## ⭐ Remember

**RBAC = Role → Permissions**
