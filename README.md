# Fortnite Battle Royale - Itemshop Guide

> [!NOTE]
> ***All Fortnite cosmetics can be found at [Fortnite.GG/Cosmetics](https://fortnite.gg/cosmetics?game=br&type=outfit&season=1,2,3,4,5,6,7,8,9,10,11,12&sort=oldest).***

---

> ### Requirements for Cosmetics
- **Version:** Must be from Chapter 2 Season 2 (Version 12.41) or earlier.
- **Pricing:** Use Fortnite’s official V-Bucks pricing.
- **Cosmetic ID:** Must follow the correct format (see below).

---

> ### Config File Structure
The item shop is defined using a JSON file. It contains slots for both daily (`daily1` to `daily6`) and featured (`featured1` to `featured4`) items, each with a `price` (in V-Bucks) and `itemGrants` (Cosmetic IDs).

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

> ### Cosmetic ID Formatting
```
ItemType:CosmeticID
```
**Examples:**
- **Skin:** `"AthenaCharacter:Example"`
- **Emote:** `"AthenaDance:Example"`
- **Pickaxe:** `"AthenaPickaxe:Example"`
- **Backbling:** `"AthenaBackpack:Example"`
- **Glider:** `"AthenaGlider:Example"`
- **Wrap:** `"AthenaItemWrap:Example"`
- **Loading Screen:** `"AthenaLoadingScreen:Example"`
- **Skydiving Contrail:** `"AthenaSkyDiveContrail:Example"`

> **Important Tip:** Always wrap Cosmetic IDs in double quotes.

---

> ### Setting Up Your Item Shop
To add an item to your shop, fill in the slot with its `itemGrants` (Cosmetic ID) and `price` (cost in V-Bucks).

#### *Output Example:*
```json
{
  "//": "BR Item Shop Config",
  "daily1": {"itemGrants": ["AthenaCharacter:CID_259_Athena_Commando_M_StreetOps"], "price": 1200},
  "daily2": {"itemGrants": ["AthenaCharacter:CID_260_Athena_Commando_F_StreetOps"], "price": 1200},
  "daily3": {"itemGrants": ["AthenaPickaxe:Pickaxe_ID_190_GolfClub"], "price": 500},
  "daily4": {"itemGrants": ["AthenaGlider:Glider_ID_176_BlackMondayCape_4P79K"], "price": 800},
  "daily5": {"itemGrants": ["AthenaBackpack:BID_229_LuckyRiderMale"], "price": 750},
  "daily6": {"itemGrants": ["AthenaItemWrap:Wrap_197_ToxinBubbles"], "price": 250},
  "featured1": {"itemGrants": ["AthenaDance:EID_FrisbeeShow"], "price": 500},
  "featured2": {"itemGrants": ["AthenaCharacter:CID_650_Athena_Commando_F_HolidayPJ_B"], "price": 800},
  "featured3": {"itemGrants": ["AthenaCharacter:CID_048_Athena_Commando_F_HolidayGingerbread"], "price": 1500},
  "featured4": {"itemGrants": ["AthenaPickaxe:Pickaxe_ID_015_HolidayCandyCane"], "price": 1500}
}
```

---

> ### Common Mistakes to Avoid
- **No Quotes:** Always put cosmetic IDs in double quotes.
- **Comma Errors:** Write numbers without commas (e.g., use `1200` not `1,200`).
- **Wrong Versions:** Do not use cosmetics from after Chapter 2 Season 2.

---

> ### Pro Tips
- **Use VS Code:** It highlights JSON errors and keeps formatting clean.
- **Validate with AI Tools:** Tools like ChatGPT can help check your JSON before testing.
