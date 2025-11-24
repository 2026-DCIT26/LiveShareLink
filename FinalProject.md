# LiveShareLink

BSCS 3-1 
https://docs.google.com/spreadsheets/d/1jvTMjXJBvBpcuqoNQT1ZUrFei92qvTTePa5ylhdnxig/edit?usp=sharing

# Project Setup Guide: GitHub & React Native (Expo)
**Course:** DCIT 26 – Application Development and Emerging Technologies  
**Tech Stack:** React Native (Expo)

This guide outlines the steps to initialize your development environment, set up your project management board, and link your code repository in compliance with the **Finals Project Documentation**.

---

## Phase 1: Set Up the "Digital Office" (GitHub Projects)

This phase addresses the **Development Timeline** and **Core Features** planning requirements.

### 1. Create the Board
1.  Log in to **GitHub**.
2.  Go to your **Profile** or **Organization**.
3.  Click the **Projects** tab $\rightarrow$ **New project**.
4.  Select **Board** (Kanban style).
5.  **Name:** `[YourAppName]-Board` (e.g., *HabitTracker-Board*).

### 2. Configure Columns
Rename the default columns to match a standard development workflow:
* **Todo (Backlog):** Your requirements list.
* **In Progress:** Features currently being coded.
* **Review/Testing:** For testing on Android/iOS simulators.
* **Done:** Completed features.

### 3. Add Initial Tasks
Add the following cards to the **Todo** column based on your project instructions:

**Core Features:**
- [ ] Identify Key Functions (e.g., CRUD operations)
- [ ] Define Data Structures
- [ ] Create Reusable Components (Headers, Modals)

**UI/UX:**
- [ ] Design Navigation Structure (Stack/Tab)
- [ ] Define Color Palette & Typography
- [ ] Implement Accessibility (Contrast/Font sizing)

---

## Phase 2: Initialize the Repository (The Code)

We will use **Expo** for this project to ensure easier testing on both Android and iOS simulators.

### 1. Create an Empty Remote Repository
1.  Click the **+** icon in the top-right corner of GitHub $\rightarrow$ **New repository**.
2.  **Name:** `[YourAppName]` (must be unique).
3.  **Description:** "React Native Expo project for DCIT 26 Finals."
4.  **Visibility:** **Public**.
5.  **CRITICAL STEP:** Do **NOT** check "Add a README," ".gitignore," or "License." The repository must be completely empty.
6.  Click **Create repository**.
7.  **Copy the HTTPS URL** provided (e.g., `https://github.com/username/repo.git`).

### 2. Initialize Local Expo App
Open your terminal (Command Prompt, PowerShell, or Terminal) and run the following commands:

```bash
# 1. Create the Expo project (Install latest version)
npx create-expo-app@latest YourAppName

# 2. Navigate into the project folder
cd YourAppName

# 3. Rename the default branch to 'main'
git branch -M main
