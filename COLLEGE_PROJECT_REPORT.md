# RAWAL INSTITUTE OF ENGINEERING AND TECHNOLOGY
## Department of Computer Science and Engineering

# Project Report
## CreatorOS — An AI-Powered Content Creation Assistant

**Submitted by:** Team TNF Code Breakers  
**Members:** Piyush, Pratham Arora, Prajwal Singh  
**Course:** B.Tech Computer Science and Engineering  
**Semester:** 3rd Semester  
**Academic session:** 2026–2027  
**Project guide:** ______________________

---

## 1. Abstract

CreatorOS is a web-based content creation assistant designed to support digital creators, student filmmakers, editors, and small creative teams. It provides a single interface for preparing content ideas, short-form video scripts, social-media captions, and production shot lists. The prototype is developed using Python and Streamlit. SQLite is used to store saved projects, while optional AI integration can generate more tailored responses when an API key and suitable model access are configured. A demo mode is also included so the application can be explored without an API key. The project demonstrates how a simple web application can combine user input, content templates, optional AI services, and local database storage.

## 2. Introduction

Digital content is published across platforms such as Instagram, YouTube, and professional social networks. Planning content may involve several tasks: choosing an idea, writing a script, drafting a caption, and deciding which shots to record. Switching between separate tools can make the planning process less organized.

CreatorOS proposes a compact workspace that combines these early-stage tasks. It is intended as an educational prototype for learning Python application development, interface design, API integration, and database operations.

## 3. Problem Statement

Creators may spend significant time organizing ideas and preparing supporting materials for a video or social post. Beginners may also find it difficult to structure a script or convert an idea into a practical shot list. A lightweight application that groups these planning tasks together can provide a more organized starting point.

## 4. Objectives

1. Build a web interface using Python.
2. Provide tools for idea generation, script drafting, caption writing, and shot planning.
3. Demonstrate optional integration with an AI service.
4. Store project outputs locally using SQLite.
5. Allow users to download generated content.
6. Practice software development, testing, documentation, and teamwork.

## 5. Scope

The initial prototype includes four content tools, a dashboard, a local database, and download support. It is suitable for demonstrating basic application development concepts. User accounts, cloud synchronization, automated scheduling, team permissions, and advanced media generation are outside the initial scope.

## 6. Technology Stack

- **Python:** Application logic.
- **Streamlit:** Web interface and user interaction.
- **SQLite:** Local storage for saved projects.
- **OpenAI API (optional):** AI-powered content generation.
- **python-dotenv:** Loading local configuration from an environment file.
- **Git/GitHub:** Recommended for source-code version control.

## 7. System Design

### Input
The user selects a tool and enters a topic, platform, duration, tone, audience, and optional instructions.

### Processing
The application checks the input. If a configured AI API is available, it sends a prompt to the model. Otherwise, it returns a clearly identified demo template.

### Output
The generated draft appears in the application and can be downloaded. The user can save it to the local SQLite database.

### Storage
Saved projects include a title, tool type, topic, platform, tone, content, and creation timestamp.

## 8. Main Modules

### 8.1 Dashboard
Displays the product identity, available tools, saved-project count, and basic guidance.

### 8.2 Idea Generator
Produces a set of starting concepts based on the selected topic.

### 8.3 Script Writer
Creates a structured script draft with a hook, story development, main moment, and ending.

### 8.4 Caption Generator
Provides caption options and a set of suggested hashtags.

### 8.5 Shot List Generator
Organizes suggested shots with framing, action, and purpose.

### 8.6 Saved Projects
Allows users to save, view, download, and delete generated drafts.

## 9. Working Methodology

1. Collect user input through the interface.
2. Validate that a topic has been entered.
3. Select demo templates or request AI-generated content.
4. Display the result.
5. Allow downloading or saving.
6. Store saved project data in SQLite.
7. Test the tools with several topics and confirm saved records can be retrieved.

## 10. Testing Plan

The team should perform and record these checks before the demonstration:

| Test | Expected result |
|---|---|
| Open the application | Dashboard loads without an error |
| Generate content with a topic | A result appears |
| Submit an empty topic | A validation warning appears |
| Run without an API key | Demo mode works |
| Save a generated result | Project appears under Saved Projects |
| Download a result | A Markdown file is downloaded |
| Delete a saved project | The project disappears from the list |
| Restart the application | Saved SQLite projects remain available |

Record actual results after testing. Do not mark a test as passed until it has been performed.

## 11. Limitations

AI mode depends on a valid API key, model access, network connectivity, and available API billing. Demo mode uses prepared templates rather than live AI. The application currently stores data locally on the computer where it runs. It does not include user authentication, cloud backup, or simultaneous collaboration.

## 12. Future Scope

Possible improvements include user accounts, team collaboration, a content calendar, storyboard planning, voice-over support, multilingual output, and cloud deployment. These should be treated as proposed improvements until implemented and tested.

## 13. Conclusion

CreatorOS is an educational prototype that demonstrates how Python, a web interface, local data storage, and optional AI integration can be combined to support content-planning workflows. It gives Team TNF Code Breakers a practical opportunity to apply foundational computer-science concepts to a creative use case.

## 14. References

1. Python documentation: https://docs.python.org/3/
2. Streamlit documentation: https://docs.streamlit.io/
3. SQLite documentation: https://www.sqlite.org/docs.html
4. OpenAI API documentation: https://platform.openai.com/docs/

---

**Important:** Add your guide's name, institution-required certificate/declaration pages, real screenshots, and actual test results before submitting. Follow the format specified by your department.
