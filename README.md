# Live Match Event Notification and Alert System
## 1. Overview
The Cricket Match Notification System is designed to provide real-time updates and insights to enhance fan engagement during live matches. The system uses predictive models, real-time data analysis, and event-triggered notifications to keep fans informed about key moments, momentum shifts, and match milestones as they unfold. The core functionality of the system is driven by an algorithm that continuously monitors the match data and triggers notifications based on significant events.

# DEMO
![Media (2)](https://github.com/user-attachments/assets/56dd91d8-17ec-4597-a2aa-77c0166f045a)

## 2. Core Features
### 2.1 Score Potential Prediction
  * **Objective**: Predict the first innings score based on early match data.
  * **Algorithm**:
    *	The model uses the average scores observed after the 7th and 8th overs.
    *	The system continuously updates the score potential based on the current match's progression.
    *	Notification is triggered when a significant change in score potential occurs.
### 2.2 Win/Loss Probability
  * **Objective**: Predict the likelihood of each team winning during the match.
  * **Algorithm**:
o	Multiple match factors and historical data are used to calculate win/loss probability.
o	The system tracks the win probability graph and triggers notifications when a significant shift occurs, indicating a possible change in match outcome.
o	Notifications are sent if the probability graph crosses a certain threshold (e.g., sudden swings indicating momentum changes).
### 2.3 Momentum Shift Detection
  * **Objective**: Detect significant momentum shifts between teams and notify spectators.
  * **Algorithm**:
    * Momentum is calculated as the difference in performance metrics (runs scored, wickets taken, boundaries, etc.) between the two teams.
    * A threshold of 15 points is used to detect a significant momentum shift.
    * Notifications are triggered when the difference in momentum between the two teams exceeds this threshold.
    * The notification includes details about the momentum shift event, such as when it occurred and which team gained the upper hand.
### 2.4 Match Milestone Notifications
  * **Objective**: Track key player and match milestones and notify fans in real-time.
  * **Algorithm**:
    * The system continuously monitors key match events, such as:
      * Batsman milestones: When a player reaches a fifty or a hundred.
      * Bowler milestones: When a bowler takes 3 wickets (a "3-fer").
      * Dot balls: When three or more consecutive dot balls are bowled.
      * Boundary events: When a boundary (four or six) follows three consecutive dot balls.
    * Notifications are triggered as soon as these milestones are reached, providing fans with timely updates.
    * The notification system ensures that milestones are not missed, increasing engagement by highlighting critical moments.
### 2.5 Game Control Function
  * **Objective**: Track the momentum and game control from over to over, notifying fans about which team is gaining the upper hand.
  * **Algorithm**:
    * The Momentum between teams is tracked from:
      * The 1st to the 8th over for the first innings.
      * The 1st to the 15th over for the second innings.
    * Notifications are sent after the 8th and 15th overs, indicating which team is in control based on the momentum data.
    * The system continuously updates the game control status, sending notifications when the team in control changes due to momentum shifts.
### 2.6 True Score Model
  * **Objective**: Predict the impact of each ball in real-time to dynamically adjust score predictions.
  * **Algorithm**:
    * Impact Scores are calculated for each delivery based on the current match context, such as the runs scored or the outcome of the ball (e.g., wicket or boundary).
    * The system updates the True Score Model within 3-5 seconds after each ball.
    * Real-time notifications are sent to fans after each significant ball event, maintaining high engagement levels by keeping spectators informed instantly.

## 3. Methodology and Workflow
The Notification System Algorithm operates based on the following workflow:
  **I.	Data Collection:** Real-time match data is collected from various sources, including player performance, team metrics, and match events (runs, wickets, overs, etc.).
  **II.	Event Detection:**
    * The algorithm continuously analyzes the incoming data to detect key events such as momentum shifts, score predictions, milestones, and game control changes.
    * If any of the predefined conditions (momentum change > 15, milestone reached, etc.) are met, a corresponding notification is triggered.
  **III.	Notification Triggering:**
    * When a significant event is detected, the system automatically generates and sends a notification to users.
    * Notifications are sent through the app or other communication channels, ensuring users are promptly informed of critical match moments.
  **IV.	Real-Time Updates:**
    * The algorithm updates in real-time as new data is received, continuously adjusting predictions and tracking game dynamics.
    * Fans are kept engaged with up-to-date information, ensuring they are informed of every significant change during the match.

## 4. Benefits of the Notification System
  * **Real-Time Engagement:** Fans are informed of key moments as they happen, maintaining high levels of engagement throughout the match.
  * **Dynamic Predictions:** The system updates predictions in real-time, providing fans with the latest match outlook, including score potential and win probability.
  * **Proactive Alerts:** Notifications about momentum shifts, milestones, and game control are sent proactively, keeping spectators informed about crucial match developments.
  * **Fan Experience:** By providing timely and relevant notifications, the system enhances the overall fan experience, ensuring they stay connected with the game's flow.

## 5. Technology Used
  * Python
  * Mysql
  * OneSignal SDK

## 6. Conclusion
The Cricket Match Notification System Algorithm is a powerful tool for enhancing fan engagement during live cricket matches. By leveraging real-time data analysis, the system provides predictive insights and immediate notifications about key events, including score changes, momentum shifts, milestones, and win/loss probabilities. The algorithm ensures that fans are always in the loop, enriching the viewing experience and making the match more immersive.
