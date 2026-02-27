# Ex03 To-Do List using JavaScript
# Name : KARTHIK G.
# Reg No : 212223220043
## Date:27.02.2026

## AIM
To create a To-do Application with all features using JavaScript.

## ALGORITHM
### STEP 1
Build the HTML structure (index.html).

### STEP 2
Style the App (style.css).

### STEP 3
Plan the features the To-Do App should have.

### STEP 4
Create a To-do application using Javascript.

### STEP 5
Add functionalities.

### STEP 6
Test the App.

### STEP 7
Open the HTML file in a browser to check layout and functionality.

### STEP 8
Fix styling issues and refine content placement.

### STEP 9
Deploy the website.

### STEP 10
Upload to GitHub Pages for free hosting.

## PROGRAM
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>AI Tasks | Smart Task Manager</title>
    <link rel="stylesheet" href="style.css">
    <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@400;600;700;800&display=swap" rel="stylesheet">
</head>
<body>

    <div class="app-shell">
        <!-- LOGIN VIEW -->
        <section id="view-login" class="view">
            <header class="hero-header">
                <div class="ai-badge">AI POWERED</div>
                <h1>TO DO LIST</h1>
                <p>AI-powered task management for students & teachers</p>
            </header>

            <div class="role-grid">
                <div class="role-card" onclick="loginRole('student')">
                    <div class="status-tag">POPULAR</div>
                    <div class="role-icon"></div>
                    <div class="role-info">
                        <h3>I am a Student</h3>
                        <p>Get study tasks & AI suggestions</p>
                    </div>
                </div>

                <div class="role-card" onclick="loginRole('teacher')">
                    <div class="role-icon"></div>
                    <div class="role-info">
                        <h3>I am a Teacher</h3>
                        <p>Plan lessons & manage class tasks</p>
                    </div>
                </div>
            </div>
        </section>

        <!-- TODO LIST VIEW -->
        <section id="view-todolist" class="view" style="display:none;">
            <div class="todo-header">
                <div style="display: flex; align-items: center; gap: 12px;">
                    <div id="role-icon-header" style="font-size: 28px;"></div>
                    <div>
                        <h1 id="role-title-header">Tasks</h1>
                        <p id="role-desc-header" style="font-size: 12px; margin: 4px 0 0 0;"></p>
                    </div>
                </div>
                <button class="logout-btn" onclick="logout()">Logout</button>
            </div>

            <!-- AI SUGGESTION INPUT -->
            <div class="ai-suggest-box">
                <h3>Get AI Task Suggestions</h3>
                <div class="suggest-options">
                    <button class="suggest-btn active" onclick="switchSuggestMode('quick')">Quick Suggestions</button>
                    <button class="suggest-btn" onclick="switchSuggestMode('custom')">Custom Input</button>
                </div>
                
                <div id="quick-suggest-mode" class="suggest-mode">
                    <button class="ai-suggest-quick-btn" onclick="getQuickSuggestions()">
                         Generate Role-Based Tasks
                    </button>
                </div>

                <div id="custom-suggest-mode" class="suggest-mode" style="display:none;">
                    <div style="display: flex; gap: 8px;">
                        <input type="text" id="task-prompt" placeholder="e.g., 'Python projects for beginners'" class="task-prompt-input">
                        <button class="ai-generate-btn" onclick="getCustomSuggestions()">Generate</button>
                    </div>
                </div>
            </div>

            <!-- LOADING STATE -->
            <div id="ai-loading" class="loading-state" style="display:none;">
                <div class="spinner"></div>
                <p>AI is generating tasks...</p>
            </div>

            <!-- ADD CUSTOM TASK -->
            <div class="add-task-box">
                <div style="display: flex; gap: 8px;">
                    <input type="text" id="task-input" placeholder="Add a new task..." class="task-input">
                    <select id="task-priority" class="task-priority">
                        <option value="low">Low</option>
                        <option value="medium" selected>Medium</option>
                        <option value="high">High</option>
                    </select>
                    <button class="add-task-btn" onclick="addTask()">Add</button>
                </div>
            </div>

            <!-- TASKS LIST -->
            <div class="tasks-container">
                <div id="tasks-list" class="tasks-list"></div>
                <div id="empty-state" class="empty-state">
                    <p>No tasks yet. Add one or get AI suggestions!</p>
                </div>
            </div>
        </section>
    </div>

    <script src="script.js"></script>
</body>
</html>
```

## OUTPUT
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/3a002e4b-9ac9-4b9c-b060-b8da04dbac8a" />
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/502c07e8-5096-4299-b50b-d07f703df6f6" />


## RESULT
The program for creating To-do list using JavaScript is executed successfully.
