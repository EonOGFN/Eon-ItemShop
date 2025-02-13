## ⚠️ IMPORTANT ⚠️
You can retrieve all Fortnite cosmetics from **[Fortnite.GG](https://fortnite.gg/cosmetics)**.

### Requirements:
1. **Cosmetics must be from Chapter 2 Season 2 (Version 12.41) or earlier.** Anything newer won’t work.
2. **Ensure V-Bucks prices match original Fortnite pricing.**
3. **Use the correct Cosmetic ID Format.** Otherwise, items will not function properly.

---

## 🔧 How to Set Up Your Item Shop

### **Step 1: Understand the Config Format**
The item shop configuration follows this structure:

```json
{
    "//": "BR Item Shop Config",
    "daily1": {"itemGrants": [""], "price": 0},
    "daily2": {"itemGrants": [""], "price": 0},
    "daily3": {"itemGrants": [""], "price": 0},
    "daily4": {"itemGrants": [""], "price": 0},
    "daily5": {"itemGrants": [""], "price": 0},
    "daily6": {"itemGrants": [""], "price": 0},
    "featured1": {"itemGrants": [""], "price": 0},
    "featured2": {"itemGrants": [""], "price": 0},
    "featured3": {"itemGrants": [""], "price": 0},
    "featured4": {"itemGrants": [""], "price": 0}            
}
```

---

### **Step 2: Use the Correct Cosmetic ID Format**
Each item in Fortnite has a **Cosmetic ID** that must follow a specific format.

#### ✅ Example:
If the **Cosmetic ID** is `Character_EonFN` and it's a skin, it must be formatted as:
```json
"AthenaCharacter:Character_EonFN"
```

#### **📌 Correct Formatting by Item Type:**
- **Skins:** `AthenaCharacter:CosmeticID`
- **Emotes:** `AthenaDance:CosmeticID` *(Includes Dances, Emoticons, Sprays)*
- **Pickaxes:** `AthenaPickaxe:CosmeticID`
- **Gliders:** `AthenaGlider:CosmeticID`
- **Wraps:** `AthenaItemWrap:CosmeticID`
- **Loading Screens:** `AthenaLoadingScreen:CosmeticID`
- **Skydiving Contrails:** `AthenaSkyDiveContrail:CosmeticID`

---

### **Step 3: Fill Out Your Item Shop**
- **`itemGrants`**: The items that will be available for purchase, identified by their **Cosmetic ID**.
- **`price`**: The cost of the item in **V-Bucks** (must match original Fortnite pricing).

#### ✅ Example Item Shop Config:
```json
{
    "//": "BR Item Shop Config",
    "daily1": {"itemGrants": ["AthenaCharacter:Character_EonFN"], "price": 1200},
    "daily2": {"itemGrants": ["AthenaPickaxe:Pickaxe_EonFN"], "price": 800},
    "daily3": {"itemGrants": ["AthenaDance:Dance_Flare"], "price": 500},
    "daily4": {"itemGrants": ["AthenaItemWrap:Wrap_Galaxy"], "price": 300},
    "daily5": {"itemGrants": ["AthenaGlider:Glider_StarSurfer"], "price": 1500},
    "daily6": {"itemGrants": ["AthenaLoadingScreen:LoadingScreen_Galactic"], "price": 200},
    "featured1": {"itemGrants": ["AthenaCharacter:Character_Drift"], "price": 2000},
    "featured2": {"itemGrants": ["AthenaDance:Dance_DefaultDance"], "price": 200},
    "featured3": {"itemGrants": ["AthenaSkyDiveContrail:Contrail_Rainbow"], "price": 400},
    "featured4": {"itemGrants": ["AthenaItemWrap:Wrap_Camo"], "price": 600}
}
```

---

### **✅ Final Checklist**
- ✔️ Ensure all cosmetics are from **Chapter 2 Season 2 (Version 12.41) or earlier**.
- ✔️ Use the **correct Cosmetic ID format**.
- ✔️ Match **V-Bucks prices** to Fortnite’s official pricing.
- ✔️ Double-check for typos in the config.
