# AI-Rules
**Repository Description:**  
Repository to define and manage custom AI rules and behaviors, supporting Windsurf and Cursor rules, organized by category and technology for tailored AI behavior and easy maintenance.

This repository provides a structured framework to **define, organize, and manage custom AI rules and behaviors** tailored to specific domains and technologies. The rules are designed to work with various AI coding assistants including Windsurf, Cursor, and other AI tools.

The repository is organized hierarchically by **category** and **technology**, making it easy to locate, add, or modify rules for specific domains.

---

## 📂 Repository Structure
The repository is organized hierarchically by **category** and **technology**:
```
ai-rules/
├── rules/
│   ├── backend/
│   │   ├── java-springboot-rules.md
│   │   └── python-fastapi-rules.md
│   └── frontend/
│       └── type-script-react-rules.md
└── README.md
```

- **Root Categories:** Broad areas like `backend`, `frontend`, `devops`, etc.
- **Rule Files:** Technology-specific rule files with consistent naming: `{technology}-rules.md`.

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
   ```bash
   git clone <repository-url>
   cd AI-Rules
   ```

### For Windsurf Users

#### Global Configuration Setup
1. **Navigate to the cloned AI-Rules directory**:
   ```bash
   cd AI-Rules
   ```
2. **Copy rules to global memories location** (replace 'YOUR_USERNAME' with your username):
   ```bash
   # For Spring Boot projects - Global configuration
   cp rules/backend/java-springboot-rules.md /Users/YOUR_USERNAME/.codeium/memories/java-springboot-rules.md
   
   # For Python FastAPI projects
   cp rules/backend/python-fastapi-rules.md /Users/YOUR_USERNAME/.codeium/memories/python-fastapi-rules.md
   
   # For React TypeScript projects
   cp rules/frontend/type-script-react-rules.md /Users/YOUR_USERNAME/.codeium/memories/type-script-react-rules.md
   ```
3. **Rules will apply** to all projects automatically
4. **Verify setup**: Ask Windsurf "What are the coding guidelines?" in any project

#### Alternative: Manual Setup via Windsurf Plugin UI
1. **Open your project** in your IDE with Windsurf plugin installed
2. **Access Windsurf Rules panel**:
   - Click on the **"Rules, Memories & Workflows"** button in Windsurf
3. **Create Global Rules**:
   - Choose the **"Rules"** tab
   - Click the **"+ Global"** button
4. **Add Rules Content**:
   - Copy the content from the appropriate `{technology}-rules.md` file
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
   - Copy the content from the appropriate technology rules file (`{technology}-rules.md`)
   - Paste it into the User Rules text area
   - **Save** the settings
4. **Rules will apply** to all projects automatically

### For Other AI Tools
Most AI coding assistants support custom rules or instructions. Simply copy the content from the appropriate `{technology}-rules.md` file and add it to your AI tool's configuration according to its documentation.

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

| Technology | Rule File Location |
|------------|-------------------|
| **Spring Boot Java** | `rules/backend/java-springboot-rules.md` |
| **FastAPI Python** | `rules/backend/python-fastapi-rules.md` |
| **React TypeScript** | `rules/frontend/type-script-react-rules.md` |

---

**Remember**: These rules are living documents that evolve with our team's needs and industry best practices. Keep them updated and provide feedback for continuous improvement!
