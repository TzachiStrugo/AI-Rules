# AI-Rules
**Repository Description:**  
Repository to define and manage custom AI rules and behaviors, supporting Windsurf and Cursor rules, organized by category and technology for tailored AI behavior and easy maintenance.

This repository provides a structured framework to **define, organize, and manage custom AI rules and behaviors** tailored to specific domains, technologies, and user preferences. It supports multiple behavior types, including:

- **Windsurf rules** – for dynamic workflow guidance.
- **Cursor rules** – for context-sensitive decision-making.

The repository is organized hierarchically by **category**, **technology**, and **rule type**, making it easy to locate, add, or modify rules for specific domains.

---

## 📂 Repository Structure
The repository is organized hierarchically by **category**, **technology**, and **rule type**:
```
ai-rules/
├── backend/
│   ├── java-springboot/
│   │   ├── windsurf/
│   │   │   └── <rule-files>
│   │   └── cursor/
│   │       └── <rule-files>
│   └── python-fastapi/
│       ├── windsurf/
│       └── cursor/
└── frontend/
    └── type-script-react/
        ├── windsurf/
        └── cursor/
```

- **Root Categories:** Broad areas like `backend`, `frontend`, `devops`, etc.
- **Subcategories:** Framework or technology-specific directories, e.g., `java-springboot`.
- **Rule Type Directories:** `windsurf/` and `cursor/` for behavior-specific rules.

---

## 🎯 Purpose

These rules help AI assistants understand our:
- **Coding standards** and best practices
- **Architecture patterns** and design principles  
- **Testing strategies** and frameworks
- **Security requirements** and guidelines
- **Technology-specific** conventions

## 🚀 Setup Instructions

### Prerequisites
1. **Clone this repository** first:
  
### For Windsurf Users

#### Global Configuration Setup
1. **Navigate to the cloned ai-rules directory**:
   ```bash
   cd ai-rules
   ```
2. **Copy rules to global memories location** (replace 'YOUR_USERNAME' with your username):
   ```bash
   # For Spring Boot projects - Global configuration
   cp backend/java-springboot/windsurf/windsurf-rules.md /Users/YOUR_USERNAME/.codeium/memories/windsurf-rules.md
   
   # Example for user 'john':
   cp backend/java-springboot/windsurf/windsurf-rules.md /Users/john/.codeium/memories/windsurf-rules.md
   ```
3. **Rules will apply** to all projects automatically
4. **Verify setup**: Ask Windsurf "What are the coding guidelines?" in any project

#### Alternative: Manual Setup via Windsurf Plugin UI
1. **Open your project** in IntelliJ IDEA with Windsurf plugin installed
2. **Access Windsurf Rules panel**:
   - Click on the **"Rules, Memories & Workflows"** button in Windsurf
3. **Create Global Rules**:
   - Choose the **"Rules"** tab
   - Click the **"+ Global"** button
4. **Add Rules Content**:
   - Copy the content from `windsurf-rules.md` file
   - Paste it into the `global_rules.md` file that opens
   - **Save** the file
5. **Rules will apply** to all projects automatically

### For Cursor Users

#### Setup via Cursor UI
1. **Open Cursor Settings**:
   - Go to **Cursor** menu → **Settings...**
   - Select **"Cursor Settings"**
2. **Navigate to Rules section**:
   - In the settings window, go to **"Rules, Memories, Commands"** section
   - Click on **"User Rules"**
3. **Add Rules Content**:
   - Copy the content from the appropriate technology language rules directory (`AGENTS.md`)
   - Paste it into the User Rules text area
   - **Save** the settings
4. **Rules will apply** to all projects automatically

## 🛠️ Usage Guidelines

### During Code Reviews
1. **Ask the AI to review** your code:
   ```
   "Please review this code against our coding standards"
   ```
2. **The AI will check** for compliance with:
   - Coding conventions
   - Security best practices  
   - Architecture patterns
   - Testing requirements

### For Code Generation
1. **Request code** with context:
   ```
   "Generate a Spring Boot REST controller for user management following our API guidelines"
   ```
2. **The AI will generate code** that follows:
   - Naming conventions
   - Error handling patterns
   - Documentation standards
   - Security requirements


### Updating Rules
1. **Propose changes** via pull request to this repository
2. **Get repository Owner approval** before merging updates
3. **Notify developers** to update their local copies
4. **Update project documentation** if needed

## 🔄 Quick Reference

### File Locations by Technology

| Technology | Windsurf Rules | Cursor Rules |
|------------|----------------|--------------|
| **Spring Boot Java** | `backend/java-springboot/windsurf/windsurf-rules.md` | `backend/java-springboot/cursor/AGENTS.md` |
| **FastAPI Python** | `backend/python-fastapi/windsurf/windsurf-rules.md` | `backend/python-fastapi/cursor/AGENTS.md` |
| **React TypeScript** | `frontend/type_script-react/windsurf/windsurf-rules.md` | `frontend/type_script-react/cursor/AGENTS.md` |
| **Angular TypeScript** | `frontend/type_script-angular/windsurf/windsurf-rules.md` | `frontend/type_script-angular/cursor/AGENTS.md` |

---

**Remember**: These rules are living documents that evolve with our team's needs and industry best practices. Keep them updated and provide feedback for continuous improvement!
