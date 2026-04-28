# 🌊 Area Creation Guide

This guide explains how to create and configure a fishing area in the system.

## 📍 Step 1: Create the Area Part

* Go to:

```id="a1x9zp"
Workspace
└── FishEngineAreas
```

* Create a new **Part** inside `FishEngineAreas`.
* Scale the part to match the area where players should be able to fish.
* Adjust the **Transparency** so it fits your game (semi-transparent is recommended).

## 🧠 Step 2: Open Area Data

* Navigate to:

```id="l0q2ms"
ServerStorage
└── fishengine_ext
    └── fishengineareadata
```

* This is where all fishing areas are registered and configured.

## ⚙️ Step 3: Define an Area

Here is the basic structure of an area:

```lua id="g7k3vn"
[1] = {
	Name = "TestArea",
	Area = FishAreas.TestArea, -- Area in workspace
	AverageFishCatchDuration = 1, -- Seconds before a fish bites
	Fishes = {1}, -- Fish available in this area
	FishChances = {
		[1] = 100
	}
},
```

## 🔍 Step 4: Variable Breakdown

### **Name**

* The display name of the area.

### **Area**

* Reference to the part located in `Workspace -> FishEngineAreas`.

### **AverageFishCatchDuration**

* Determines how long (in seconds) it takes for a fish to bite on average.

### **Fishes**

* A list of fish IDs that can be caught in this area.

### **FishChances**

* Defines the probability of catching each fish.

## 🎯 Step 5: Setting Fish Chances

* Each fish in `Fishes` should have a corresponding entry in `FishChances`.
* The total should equal **100** for proper probability distribution.

### Example:

```lua id="n4p8td"
FishChances = {
	[1] = 70,
	[2] = 10,
	[3] = 20
}
```

* Fish 1 → 70% chance
* Fish 2 → 10% chance
* Fish 3 → 20% chance

⚠️ Make sure the total adds up to **exactly 100**.

## ✅ Done!

Your fishing area is now configured and ready to use in the system.
