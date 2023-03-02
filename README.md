# GemScape (2D)

GemScape is a game that takes place in the enchanted world of Arcania. 

Read more on our [documentation](https://docs.adv3nture.xyz/introduction/gemscape).

## Principles

1. Open
- Free-to-play - anyone can play

2. Interoperable & Composable
- NFTs & ERC-20 tokens that can be used across different games
    - E.g. Same character (NFT) can be used across different games
- Omni-chain

3. Collaborative
- 3rd-party NFT communities get an in-game avatar based on their PFP
- Features that promote teamwork and collaboration e.g. boss raids

## Gameplay

### Character Schema

```javascript
Player {
    character: {
        level: 1,
        xp: 0,
        race: "Human"
        class: "",
    },
    attributes: {
        strength: 10,
        agility: 10,
        wisdom: 10,
        constitution: 10,
        luck: 10,
        intuition: 10,
        perception: 10,
    },
    skills: {
        mining: xpMining,
        crafting: xpCrafting,
        farming: xpFarming,
    },
    equipment: {
        head: "",
        body: "",
        weapon: "",
        legs: "",
    }
}
```

- STR determines attack damage
- AGI determines and dodge chance
- WIS determines critical attack chance

### V1 Features

1. Mining

Stake character for 24h to earn:
- $GEM tokens
- XP for Mining Skill

2. Questing
- $GOLD tokens
- XP for Character Level
- Drops for crafting items (e.g. leather, thread)

3. Crafting

Craft a Gemstone Broadsword:
- x $GEM tokens
- x $GOLD tokens
- x level mining
- x leather

4. Farming / Gardening

-> plant something
- e.g. Deposit LP tokens (GEM/ETH or GOLD/USDC) 

-> earn rewards
- e.g. GEM or GOLD tokens
- rewards vested e.g. over 6 months

5. Grand Exchange

a) DEX interface to trade tokens:
- 0x API for trading on DEX?
- dex interface to buy/sell GEM and GOLD tokens

b) Bank
- stake GEM to get xGEM (or GOLD to get xGOLD)
- GEM (and GOLD) added to the bank contract from fees i.e. xGEM holders get more GEM over time
- xGEM & xGOLD holders get voting rights in DAO

6. View Character / Profile
- Stats
- Show inventory
- Show tokens and NFTs

7. Equip NFTs to Character:
- Weapons and other equipment
- NFTs for special boosts
    - e.g. ADV NFT to get extra stats from NFT added to character

8. Upgradeable contract (?)

### V2 Features

1. Dungeon Run
Single-player activity 
or battling (farming items etc)

2. Battle Boss
Multiplayer / collaborative activity

## References

Inspired by:
- DeFi Kingdoms
- Loot Project
- RuneScape
