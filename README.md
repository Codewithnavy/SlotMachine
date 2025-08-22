# 🎰 Slot Machine – Unity Project  

## 📖 Overview  
This project is a **Unity-based Slot Machine game**, built as a learning exercise to explore **game mechanics, object-oriented programming in C#, and shader usage in Unity**.  
It represents one of my **first complete projects** in game development and showcases the ability to design, structure, and deploy a functional interactive game.  

---

## 🎯 Objectives  
- Understand **Unity game engine workflows**.  
- Apply **C# scripting** for game mechanics.  
- Implement **UI/UX elements** for interactive play.  
- Explore **ShaderLab** for visual enhancements.  
- Learn **basic probability logic** for slot outcomes.  

---

## 🛠️ Tech Stack  
- **Engine:** Unity  
- **Languages:**  
  - C# (Game Logic)  
  - ShaderLab & HLSL (Graphics/Effects)  

---

## ✨ Features  
- 🎰 Slot machine with reels and spin functionality.  
- 💡 Simple but extendable probability system.  
- 🎨 Custom shaders for reel visuals.  
- 📊 Clean project structure for easy understanding.  

---

## 📐 UML Class Diagram  

```mermaid
classDiagram
    class GameManager {
        - int coins
        - Reel[] reels
        + StartGame()
        + Spin()
        + CheckWin()
    }

    class Reel {
        - string[] symbols
        + SpinReel() string
    }

    class UIManager {
        + UpdateCoins(int)
        + ShowResult(string)
    }

    GameManager --> Reel
    GameManager --> UIManager
