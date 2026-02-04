# Enhanced Task Tracker

A productivity-focused web application that combines task management with gamification elements to encourage daily consistency.

## 🌟 Key Features

* **Gamified Streak System:** Tracks consecutive days of task completion using `localStorage`.
* **Dynamic Dark Mode:** A fully themed dark interface that persists across browser sessions.
* **Animated Feedback:** A custom CSS checkmark animation triggers upon task completion to provide positive reinforcement.
* **Persistent Storage:** Tasks and user preferences (Dark Mode, Streaks) are saved locally, so data isn't lost on refresh.
* **Responsive UI:** Built with the **Inter** font family and flexible CSS for a modern, "app-like" feel.

## 🛠️ Technical Breakdown

### Streak Logic
The streak counter follows a time-sensitive validation logic:
1.  **Continuous:** If the last completion was *yesterday*, the streak increments ($S + 1$).
2.  **Reset:** If the last completion was *before yesterday*, the streak resets to 1.
3.  **Daily Cap:** Multiple tasks completed on the same day do not increment the streak further.



### UI Components
| Component | Technology | Purpose |
| :--- | :--- | :--- |
| **Checkmark** | CSS Keyframes | Provides "Frictionless Reward" via `fadeInScale` and `pulse` animations. |
| **Dark Mode** | JavaScript Class Toggling | Switches root variables for background and text colors. |
| **Task List** | DOM Manipulation | Dynamically renders `<li>` elements based on an array of objects. |

## 🚀 How to Run
1.  Save the code as `index.html`.
2.  Open the file in any modern web browser.
3.  Add your first task and hit "Complete" to see the streak logic in action!

## 🚧 Planned Improvements
- [ ] **Categorization:** Tags for "Work", "Personal", and "Health".
- [ ] **Sound Effects:** Audio cues for task completion.
- [ ] **Export Data:** Option to download task history as a JSON file.

---
*Stay productive and keep the streak alive!*
