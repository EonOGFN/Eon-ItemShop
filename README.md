## ⚠️ **IMPORTANT INFO BEFORE YOU START** ⚠️  
- You can get all Fortnite's Battle Royale cosmetics from **[Fortnite.GG](https://fortnite.gg/cosmetics)**.

### 🔑 **Requirements for Cosmetics to Work**
1. **Cosmetics must be from Chapter 2 Season 2 (Version 12.41) or earlier, Anything newer won’t work.**
2. **Set prices according to Fortnite’s original V-Bucks pricing.**  
3. **Follow the correct Cosmetic ID format.**  *Incorrect formatting will break the shop.**

---

### 🛠️ **PART 1: Understanding the Config File Structure**  
- The item shop uses a **JSON file** to define which items appear and their prices. Here's what the basic structure looks like:

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
### 🔍 **Breaking Down the Code:**
- **`daily1`, `daily2`, etc.:** Slots for daily items (up to 6 items).  
- **`featured1`, `featured2`, etc.:** Slots for featured items (up to 4 items).  
- **`itemGrants`:** The actual items being sold, identified by their **Cosmetic ID**.  
- **`price`:** How many V-Bucks the item costs.  
---

### 🏷️ **PART 2: Correct Cosmetic ID Formatting**  
- Each item has a unique ID called a **Cosmetic ID**. The format depends on the item type.

### ✅ **General Format:**  
```
ItemType:CosmeticID
```

### 🔖 **Examples by Item Type:**  
- **Skins:** `AthenaCharacter:Character_EonFN`  
- **Emotes (Dances, Emoticons, Sprays):** `AthenaDance:Dance_Flare`  
- **Pickaxes:** `AthenaPickaxe:Pickaxe_EonFN`  
- **Gliders:** `AthenaGlider:Glider_StarSurfer`  
- **Wraps:** `AthenaItemWrap:Wrap_Galaxy`  
- **Loading Screens:** `AthenaLoadingScreen:LoadingScreen_Galactic`  
- **Skydiving Contrails:** `AthenaSkyDiveContrail:Contrail_Rainbow`  

**💡 NOTE:** Always wrap your **Cosmetic ID** in double quotes (`""`), or the config will break.

---

### 🏪 **PART 3: Filling Out Your Item Shop**  
- Here’s how to set up each item in your shop:  

- **`itemGrants`:** Add the formatted Cosmetic ID for the item you want to sell.  
- **`price`:** Set the cost using Fortnite’s official V-Bucks prices.  

### ✅ **Example Config Setup:**  
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

## 🚫 **PART 4: Common Mistakes to Avoid**  

🔴 **DON’T:**  
- ❌ Forget double quotes around your **Cosmetic ID**. Example: `AthenaCharacter:Character_EonFN` → `"AthenaCharacter:Character_EonFN"`  
- ❌ Add commas to numbers. Use `1200`, not `1,200`.  
- ❌ Use cosmetics from versions after **Chapter 2 Season 2** (*they won’t work.*)

✅ **DO:**  
- ✔️ Double-check every **Cosmetic ID** format.  
- ✔️ Match Fortnite’s original V-Bucks prices.  
- ✔️ Use **Visual Studio Code** to spot errors automatically.  

---

## 💡 **PART 5: Pro Tips for a Smoother Setup**  

1. 🖥️ **Install Visual Studio Code (VS Code):**  
   - It highlights errors in your JSON automatically.  
   - Helps keep formatting clean and consistent.  

2. 🤖 **Use AI tools (like ChatGPT) to validate your JSON:**  
   - Quickly check if your formatting is correct before testing in-game.  
