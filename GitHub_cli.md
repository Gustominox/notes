### **Create a New Issue**
To create a new issue, use the following command:
```sh
gh issue create --title "Issue Title" --body "Detailed description of the issue."
```

### **Additional Options**
- **Assign an issue to someone**:  
  ```sh
  gh issue create --title "Bug: App Crashes" --body "The app crashes when clicking save." --assignee username
  ```
- **Set a label**:  
  ```sh
  gh issue create --title "New Feature Request" --body "It would be great to have a dark mode." --label "enhancement"
  ```
- **Set a milestone**:  
  ```sh
  gh issue create --title "Fix login issue" --body "Users are unable to log in." --milestone 1
  ```
- **Open in browser to edit before submission**:  
  ```sh
  gh issue create --title "Check performance" --body "Investigate memory usage." --web
  ```