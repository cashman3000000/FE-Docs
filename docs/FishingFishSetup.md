# 🐟 Fish Creation Guide

This guide explains how to create and register a fish for the fishing system.

## 📦 Step 1: Create the Fish Model

* Create a new **Model** for your fish.
* This model will contain all parts that make up the fish.

## 🛠️ Step 2: Create the Tool

* Create a **Tool** instance.
* Place the fish model inside the Tool.

## 🔩 Step 3: Weld the Fish

* Weld all parts of the fish together.
* ✅ Use **`WeldConstraint`** for all welds
* ❌ Do **NOT** use `Weld`

## 📁 Step 4: Store the Fish Model

Move the completed fish tool to:

```
ReplicatedStorage
└── fishengine_ext
    └── models
        └── fish
```

## 🧠 Step 5: Register the Fish

* Navigate to:

```
ServerStorage
└── fishengine_ext
    └── fishenginefishdata
```

* Add a reference to your fish in this data module so it can be used in the system.

## ✅ Done!

Your fish is now ready to be used in the fishing system.
