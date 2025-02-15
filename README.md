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
    "daily1": {"itemGrants": ["AthenaCharacter:EID_KPopDance03"], "price": 500},
    "daily2": {"itemGrants": ["AthenaPickaxe:Pickaxe_ID_154_Squishy"], "price": 500},
    "daily3": {"itemGrants": ["AthenaCharacter:CID_586_Athena_Commando_F_PunkDevil"], "price": 1,200},
    "daily4": {"itemGrants": ["AthenaGlider:Glider_ID_116_PizzaPit"], "price": 1,200},
    "daily5": {"itemGrants": ["AthenaCharacter:CID_344_Athena_Commando_M_IceCream"], "price": 1,500},
    "daily6": {"itemGrants": ["AthenaDance:EID_Floss"], "price": 300},
    "featured1": {"itemGrants": ["AthenaCharacter:CID_745_Athena_Commando_M_RavenQuill"], "price": 1,500},
    "featured2": {"itemGrants": ["AthenaDance:EID_Cyclone"], "price": 500},
    "featured3": {"itemGrants": ["AthenaCharacter:CID_605_Athena_Commando_M_TourBus"], "price": 1,500},
    "featured4": {"itemGrants": ["AthenaDance:EID_TourBus"], "price": 300}            
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
    "daily1": {"itemGrants": ["AthenaCharacter:EID_KPopDance03"], "price": 500},
    "daily2": {"itemGrants": ["AthenaPickaxe:Pickaxe_ID_154_Squishy"], "price": 500},
    "daily3": {"itemGrants": ["AthenaCharacter:CID_586_Athena_Commando_F_PunkDevil"], "price": 1,200},
    "daily4": {"itemGrants": ["AthenaGlider:Glider_ID_116_PizzaPit"], "price": 1,200},
    "daily5": {"itemGrants": ["AthenaCharacter:CID_344_Athena_Commando_M_IceCream"], "price": 1,500},
    "daily6": {"itemGrants": ["AthenaDance:EID_Floss"], "price": 300},
    "featured1": {"itemGrants": ["AthenaCharacter:CID_745_Athena_Commando_M_RavenQuill"], "price": 1,500},
    "featured2": {"itemGrants": ["AthenaDance:EID_Cyclone"], "price": 500},
    "featured3": {"itemGrants": ["AthenaCharacter:CID_605_Athena_Commando_M_TourBus"], "price": 1,500},
    "featured4": {"itemGrants": ["AthenaDance:EID_TourBus"], "price": 300}
}
```

---

### **✅ Final Checklist**
- ✔️ Ensure all cosmetics are from **Chapter 2 Season 2 (Version 12.41) or earlier**.
- ✔️ Use the **correct Cosmetic ID format**.
- ✔️ Match **V-Bucks prices** to Fortnite’s official pricing.
- ✔️ Double-check for typos in the config.
