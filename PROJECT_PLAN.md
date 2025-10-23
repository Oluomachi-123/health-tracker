# 🏃‍♂️ Personal Health Tracker - Project Plan

## 1. Problem Description
Many people find it difficult to consistently monitor their daily health habits such as water intake, sleep, and exercise. Manual tracking methods (notebooks or spreadsheets) are time-consuming and prone to error.

## 2. How the Program Solves the Problem
The app simplifies tracking by offering:
- A web interface to log daily data
- LocalStorage-based automatic data saving
- BMI calculator and progress charts

## 3. Requirements for the Program
### Functional Requirements
- Add, view, and summarize records (water, sleep, exercise)
- Calculate BMI and show category
- Display interactive progress charts

### Non-Functional Requirements
- Work offline
- Be mobile-friendly and responsive
- Save data locally in browser storage

## 4. How the Program Changes the Operating Model
Before: Manual data entry via spreadsheets.  
After: Automated data entry, visualization, and health insights.

## 5. Usage Context and Requirements
- Runs locally in any web browser
- No server or database required
- Suitable for personal use or small-scale wellness tracking

## 6. Software Architecture
Frontend-only system with these layers:
```
HTML/CSS (UI) → JavaScript (Logic) → LocalStorage (Data)
```
Uses Chart.js for charts and Font Awesome for icons.

## 7. Ensuring Correct Functioning
- Input validation
- Persistent data storage
- Manual testing for add/view/summary/chart features

## 8. Usability Considerations
- Simple navigation with icons
- Responsive layout
- Clear feedback and messages

## 9. Instructions for Use
1. Open `index.html` in a browser.
2. Add entries in “Add Entry.”
3. View data in “Records.”
4. See averages in “Summary.”
5. Calculate BMI in “BMI.”
6. Generate charts in “Charts.”

## 10. Technologies Used
HTML, CSS, JavaScript, Chart.js, Font Awesome

