# Project Documentation & Setup Guide: React Native (Expo)
**Course:** DCIT 26 – Application Development and Emerging Technologies  
**Instructor:** Godwin Lorenz B. Llabres  
**Timeline:** Nov 16, 2024 – Finals Week  

This guide outlines the steps to initialize your development environment, set up your project management board, and link your code repository to meet the **Finals Project Documentation** requirements.

---

## Phase 1: Set Up the "Digital Office" (GitHub Projects)
*Goal: Fulfill the "Development Timeline" and planning requirements.*

### 1. Create the Board
1.  Log in to **GitHub**.
2.  Go to your **Profile** or **Organization**.
3.  Click the **Projects** tab (top navigation bar) $\rightarrow$ **New project**.
4.  Select **Board** (Kanban style).
5.  **Name:** `[YourAppName]-Board` (e.g., *HabitTracker-Board*).

### 2. Configure Columns
Rename the default columns to match a standard development workflow:
* **Todo (Backlog):** Your requirements list (from the project instructions).
* **In Progress:** Features currently being coded.
* **Review/Testing:** For testing functionality on simulators.
* **Done:** Completed features.

### 3. Add Initial Tasks (Cards)
Add the following cards to the **Todo** column immediately based on the project requirements:

**Core Features:**
- [ ] Identify Key Functions (e.g., Habit creation, Expense categorization)
- [ ] Define Data Structures (State management/Storage)
- [ ] Create Reusable Components (Headers, Modals, Buttons)

**UI/UX:**
- [ ] Design Navigation Structure (Stack/Tab/Drawer)
- [ ] Define Color Palette & Typography (Minimal & Consistent)
- [ ] Implement Accessibility Features (Contrast checks)

---

## Phase 2: Initialize the Repository (The Code)
*Goal: Specific "Allowed end-product" setup using Expo.*

### 1. Create an Empty Remote Repository
1.  Click the **+** icon in the top-right corner of GitHub $\rightarrow$ **New repository**.
2.  **Name:** `[YourAppName]` (must be unique).
3.  **Description:** "React Native Expo project for DCIT 26 Finals."
4.  **Visibility:** **Public**.
5.  **CRITICAL STEP:** Do **NOT** check "Add a README," ".gitignore," or "License." The repository must be completely empty so we can push our local Expo code into it without conflicts.
6.  Click **Create repository**.
7.  **Copy the HTTPS URL** provided (e.g., `https://github.com/username/repo.git`).

### 2. Initialize Local Expo App
Open your terminal (Command Prompt, PowerShell, or VS Code Terminal) and run the following commands:

```bash
# 1. Create the Expo project (Installs the latest stable version)
npx create-expo-app@latest YourAppName

# 2. Navigate into the project folder
cd YourAppName

# 3. Rename the default branch to 'main' (Standard practice)
git branch -M main
