# 🎣 Rod Creation Guide
This guide walks you through the process of creating and registering a rod for the fishing system.
## 📦 Step 1: Create the Rod Model
* Create a new **Model** for your rod.
* This will serve as the main container for all rod components.
## 🛠️ Step 2: Create the Tool
* Create a **Tool** instance.
* Place your rod model inside the Tool.
* Ensure the rod is properly positioned and oriented.
## 🔩 Step 3: Weld the Rod
* Weld all parts of the rod together.
* ✅ **Important:** Use **`WeldConstraint`**
* ❌ Do **NOT** use `Weld`
## 🪝 Step 4: Add the Hook
* Create a part named **`Hook`**.
* Position it at the tip of the rod (or wherever appropriate).
* Weld it properly to the rod.
## 🎯 Step 5: Add Reel Position
* Create another part named **`ReelPosition`**.
* Place it where the reel should be located.
* Ensure it is welded to the rest of the rod.
## 📌 Step 6: Final Checks
* Make sure:
  * All parts are welded together
  * All welds are **WeldConstraints**
  * The structure is clean and organized inside the Tool
## 📁 Step 7: Store the Rod Model
Move your completed rod model to:
```
ReplicatedStorage
└── fishengine_ext
    └── models
        └── rods
```
## 🧠 Step 8: Register the Rod
* Navigate to:
```
ServerStorage
└── fishengine_ext
    └── fishengineroddata
```
* Add a reference to your rod in this data module so the system recognizes it.
## ✅ Done!
Your rod should now be fully set up and ready to use in the system.
