# 5. Availability Zones

## Definition

Availability Zones are **physically separate locations within an Azure region**, each with independent **power, cooling, and networking**.

## Why?

They **protect applications from failures affecting one datacenter**.

## Example

Your application runs:

```text
Region
├── Zone 1 → VM
├── Zone 2 → VM
└── Zone 3 → VM
```

If **Zone 1 fails**, workloads in other zones can continue.

## When to Use

Use Availability Zones when we need **high availability and protection from datacenter-level failures**.

## ⭐ Remember

**Region** → **Geographic area**

**Availability Zone** → **Separate physical location inside a region**
