# Task Explanation: Jenkins CI/CD for JavaScript Applications

## This is a Jenkins Freestyle Project for Todo List App 

### Step 1: Fork the Repository: (https://github.com/sanoojes/simple-todo-app).


### Step 2: Install Jenkins
1. Refer to the official Jenkins installation guide for your operating system: [Jenkins Installation](https://www.jenkins.io/doc/book/installing/) or these articles  [Linux](https://www.digitalocean.com/community/tutorial-collections/how-to-install-jenkins), [Windows](https://phoenixnap.com/kb/install-jenkins-on-windows) and [macOS](https://www.jenkins.io/download/lts/macos/) 
2. Follow the instructions to install Jenkins.
3. Once installed on my windows system, on my web browser, I opened `http://localhost:8080` to access Jenkins.
   
### Step 3: Create a Jenkins Freestyle Project
1. I clicked on "New Item".
2. I picked "Freestyle project".
3. Named the job "Build Todo App".
   
### Step 4: Configure Source Control
1. On source Code Management:
2. I picked "Git" and enter the URL of the forked repository

### Step 5: Add Build Steps
1. Added an "Execute Windows batch command" build step.
2. In the command box, I added the command to build your app.

```bash
echo "Building HTML/CSS/JS Project"
```
### Step 6: Archive the Build Artifacts
1. For Post-build Actions:
2. I added a post-build action to "Archive the artifacts".
3. Specified the files to archive. 
```plaintext
*.html, *.css, *.js   # This will archive all files in the workspace
```
### Step 7: Save and Verify Build
1. Saved the Job.
2. Clicked on "Build Now" to run the job and build the todo application.
3. After the build completed, I checked the console output for any errors but none.
4. Accessed the archived artifacts from the build's page in Jenkins to see the files generated during the build process.



### Yayyy! so exciting stuff!!!💪🏽🚀
