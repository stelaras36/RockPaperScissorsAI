# RockPaperScissorsAI 🎮

Rock–Paper–Scissors game in **Java** with a simple **AI that learns your moves** and a clean **Swing GUI**.  
Includes both a **runnable JAR** and a **Windows .EXE** (built with Launch4j).

---

## 🚀 Features

- ✅ Modern Swing UI (Nimbus look & feel)
- ✅ Buttons for **Rock / Paper / Scissors / Reset / Rules / About**
- ✅ Live scoreboard:
  - Rounds played
  - Player wins
  - Computer wins
  - Ties
- ✅ **Simple learning AI**:
  - Παρακολουθεί πόσο συχνά παίζεις Rock / Paper / Scissors
  - Μετά από μερικούς γύρους προσπαθεί να **αντικρούσει την πιο συχνή σου κίνηση**
- ✅ “Rules” popup με τους κανόνες του παιχνιδιού και περιγραφή του AI
- ✅ “About” popup με στοιχεία δημιουργού (Stelios Kyrikos)

---

## 🧠 How the AI works (short version)

The AI is **frequency-based**:

1. Μετράει πόσες φορές έχεις παίξει:
   - `ROCK`
   - `PAPER`
   - `SCISSORS`
2. Αν δεν έχει αρκετά δεδομένα (π.χ. < 3 κινήσεις), παίζει **random**.
3. Όταν έχει αρκετές κινήσεις:
   - Αν παίζεις πιο συχνά **ROCK** → ο υπολογιστής παίζει **PAPER**
   - Αν παίζεις πιο συχνά **PAPER** → παίζει **SCISSORS**
   - Αν παίζεις πιο συχνά **SCISSORS** → παίζει **ROCK**

Έτσι το παιχνίδι προσαρμόζεται στα patterns του παίκτη και γίνεται πιο δύσκολο όσο συνεχίζεις.

---

## 📥 Downloads

Μπορείς να κατεβάσεις έτοιμα binaries από τα **Releases**:

➡️ [Download latest release](../../releases/latest)

Στο release θα βρεις:

- `RockPaperScissorsAI.exe` – Windows executable, **δεν χρειάζεται εγκατάσταση** (απαιτεί Java στο σύστημα).
- `RockPaperScissorsAI.jar` – runnable JAR για οποιοδήποτε λειτουργικό με Java 17+.

---

## ▶️ How to run

### Option A – Windows .EXE

1. Κατέβασε το `RockPaperScissorsAI.exe` από το [latest release](../../releases/latest).
2. Κάνε **διπλό κλικ**.
3. Αν εμφανιστεί προειδοποίηση από antivirus / SmartScreen, απλά επέλεξε “Run anyway” (το exe είναι φτιαγμένο με Launch4j από το JAR).

### Option B – Runnable JAR

1. Βεβαιώσου ότι έχεις **Java 17+** εγκατεστημένη.
2. Κατέβασε το `RockPaperScissorsAI.jar`.
3. Από terminal / cmd:

```bash
java -jar RockPaperScissorsAI.jar

🧩 Technologies Used

Language: Java 17

GUI: Swing (JFrame, JButton, JLabel, layouts)

Look & Feel: Nimbus

Build / Packaging:

Runnable JAR από Eclipse

Windows EXE με Launch4j

Architecture:

Game – main UI & game flow

GameAI – frequency-based AI

GameStats – rounds, wins, ties

Move & Result enums – καθαρές αναπαραστάσεις κινήσεων & αποτελέσματος

![Main UI]
<img width="710" height="338" alt="Στιγμιότυπο οθόνης 2025-12-03 204909" src="https://github.com/user-attachments/assets/836ef4b0-9add-4d98-8994-e0657ccf4991" />
![Rules popup]
<img width="705" height="342" alt="Στιγμιότυπο οθόνης 2025-12-03 205046" src="https://github.com/user-attachments/assets/4ef2cd56-5a6a-415a-ad14-95072f69f838" />

📌 Possible future improvements

🔹 Δεύτερο επίπεδο AI (predictive patterns / Markov chain)

🔹 Χρώματα / icons για τις επιλογές Rock / Paper / Scissors

🔹 Ήχοι για win / lose / tie

🔹 Επιπλέον στατιστικά (win rate, streaks, graphs)

🔹 Localization (English / Greek UI switch)

👤 Author

Stelios Kyrikos
Computer Science student – IST College

LinkedIn: https://www.linkedin.com/in/stelioskyrikos/

GitHub: https://github.com/stelaras36

