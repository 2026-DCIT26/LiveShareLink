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
```

### 3. Push Local Code to GitHub
Connect your local Expo files to the empty GitHub repository you just created:

```bash
# 1. Link the remote repository (Paste your specific URL below)
git remote add origin https://github.com/YourUsername/YourAppName.git

# 2. Push the initial code
git push -u origin main
```

> **Note:** If the push is successful, refresh your GitHub repository page. You should now see your Expo file structure (`app`, `package.json`, `assets`, etc.).

---

## Phase 3: Link Repository to Project Board
*Goal: Link your planning (Board) with your execution (Code).*

1. Go back to your GitHub **Project Board**.
2. Click the **Settings** icon (top right, `...` or gear icon).
3. Select **Linked repositories** from the sidebar.
4. Click **Link a repository**.
5. Search for your specific repository name (`YourAppName`) and select it.

---

## Phase 4: Development Workflow
*Goal: Maintain "Efficient Functionality" throughout the semester.*

Follow this cycle for every feature until Finals Week:

1. **Select Task:** Go to your Board and drag a card (e.g., "Create Login Screen") from **Todo** to **In Progress**.

2. **Code:** Implement the feature in VS Code. Focus on **Modularization** (keep components small).

3. **Test:**
   - Run `npx expo start` in your terminal.
   - Press `a` for Android or `i` for iOS (or scan the QR code with your phone) to ensure the app behaves consistently.

4. **Save & Push:** Run the following commands to save your progress to the cloud:

   ```bash
   git add .
   git commit -m "Implemented [Feature Name]"
   git push
   ```

5. **Complete:** Drag the card on your Board to **Done**.
