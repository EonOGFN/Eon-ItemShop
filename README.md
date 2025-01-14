You can retrieve all Fortnite cosmetics from **[Fortnite.GG](https://fortnite.gg/cosmetics)**. 
Ensure they are from **Chapter 2 Season 2 (Version 12.41)** or earlier, as anything newer won’t work. Also, make sure V-Bucks Prices match those in the original Fortnite.

#### Item-Shop Config Format
```json
{
    "//": "BR Item Shop Config",
    "daily1": {"itemGrants": ["AthenaCharacter:CID_207_Athena_Commando_M_FootballDudeA"], "price": 1,500},
    "daily2": {"itemGrants": ["AthenaCharacter:CID_239_Athena_Commando_M_FootballDudeD"], "price": 1,500},
    "daily3": {"itemGrants": ["AthenaCharacter:CID_210_Athena_Commando_F_FootballGirlA"], "price": 1,500},
    "daily4": {"itemGrants": ["AthenaCharacter:CID_211_Athena_Commando_F_FootballGirlB"], "price": 1,500},
    "daily5": {"itemGrants": [""], "price": 0},
    "daily6": {"itemGrants": [""], "price": 0},
    "featured1": {"itemGrants": ["AthenaPickaxe:Pickaxe_ID_094_Football"], "price": 800},
    "featured2": {"itemGrants": ["AthenaPickaxe:Pickaxe_ID_096_FootballReferee"], "price": 500},
    "featured3": {"itemGrants": ["AthenaPickaxe:Pickaxe_ID_095_FootballTrophy"], "price": 500},
    "featured4": {"itemGrants": ["AthenaGlider:Glider_ID_071_Football"], "price": 500}            
}
```  

#### Cosmetic ID Format
The **Cosmetic ID** is the unique identifier for the item (skin, emote, etc.). To make it work in-game, it **must** use the correct format.  

#### Example:
If the **Cosmetic ID** is `Character_EonFN` and it's a skin, use: `AthenaCharacter:Character_EonFN`  

#### Formats:
- **Skins:** `AthenaCharacter:CosmeticID`  
- **Emotes:** `AthenaDance:CosmeticID`  *(Dances, Emoticons, Sprays)*
- **Pickaxes:** `AthenaPickaxe:CosmeticID`  
- **Gliders:** `AthenaGlider:CosmeticID`  
- **Wraps:** `AthenaItemWrap:CosmeticID`  
- **Loading Screens:** `AthenaLoadingScreen:CosmeticID`  
- **Skydiving Contrails:** `AthenaSkyDiveContrail:CosmeticID` 

---

- **itemGrants**: This defines the item(s) that will appear in the **Item Shop** for players to purchase. Each item is identified by its **Cosmetic ID**, which must be formatted correctly (e.g., `AthenaCharacter:CosmeticID` for skins).
  
- **price**: This specifies the cost of the item in **V-Bucks** as it will be shown in the **Item Shop**. Ensure the prices match Fortnite's official pricing.  

#### Example Config
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
