Game Title: SPIRIT HATCH

Game Type: [Tamagotchi]

Win Condition:
[The player successfully raises their spirit animal through all evolution stages by keeping its hunger, 
happiness, and health above critical levels for a set number of in-game days. A full win occurs when the pet reaches its final evolved form.]

Lose Condition:
[If hunger, health, or happiness drops to zero, the spirit animal fades and the game ends. No tie condition.]

Core Mechanics (3–5 features that MUST work):
1. Feed the spirit animal to restore hunger and health  
2. Play/interact to increase happiness  
3. Time-based stat decay (needs attention over time)  
4. Evolution system triggered by good care  
5. Status display showing all stats  


## Player Input

**Commands:**  
`feed` · `play` · `rest` · `status` · `evolve` · `help` · `quit`

---

## Inputs We Will Validate (QA Test Ideas)

- Invalid command (random letters)  
- Repeated actions when stats are already max  
- Negative or impossible stat values  
- Attempting to evolve too early  
- Empty input  

---

## Known Limitations

- Text-only interface, no graphics or animations  
- No multiplayer or online saving  
- Simple AI behavior (no complex personality system)  
- Limited number of evolution stages  

---

## Tech Stack

Python in terminal
