# Multiplayer Quiz Game

## 🎮 Introduction
This is a fun multiplayer quiz game where players take turns asking and answering questions to determine the Queen. The game supports 3 or more players who must be connected to the same WiFi network.

## 🚀 How to Play
1. Connect at least **3 devices** to the **same WiFi network**.
2. One player runs the **Game Server**.
3. Other players run the **Game Client** and join the server.
4. Each round, one player is the **Judge** and asks a question.
5. Other players, called **Knights**, answer the question.
6. **One player is randomly assigned as the Queen**.
7. The Judge selects the Queen based on the answers.
8. Wrong answers receive penalties.
9. Roles shift in each round.

## 📌 Getting Started

### 1️⃣ Clone the Repository
```sh
git clone https://github.com/ISMadusanka/emitation_game_be.git
cd emitation_game_be
```

### 2️⃣ Build the Project Using Maven
Ensure you have **Maven** installed, then navigate to the project directory and run:
```sh
mvn clean install
```

### 3️⃣ Run the Game
#### Start the Game Server
Run the following command on one device:
```sh
java -jar target/emitation_game_be-1.0-SNAPSHOT.jar --server
```
The **IP address** will be displayed in the console. **Write it down**, as it is needed to connect clients.

#### Start the Game Clients
On all other devices, run:
```sh
java -jar target/emitation_game_be-1.0-SNAPSHOT.jar --client
```
Enter the **IP address** displayed on the server console.

### 4️⃣ Modify Game Settings
The default game has **2 rounds**. You can modify the number of rounds in `GameServer.java`:
```java
private static final int MAX_ROUNDS = 6; // Change this value as needed
```

## 🏆 Have Fun!
Enjoy playing the Multiplayer Quiz Game! 👑
