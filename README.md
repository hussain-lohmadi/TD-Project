# Chronos - Time Management Redefined
![interface](https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.freepik.com%2Fpremium-vector%2Ftask-manager-planner-organizer-application-dashboard-ui-with-task-performance-process-time-management-web-app-vector-template_26839957.htm&psig=AOvVaw33YD1z92jNd0a4XM1qMNLb&ust=1729720463161000&source=images&cd=vfe&opi=89978449&ved=0CBQQjRxqFwoTCKCDsoD9ookDFQAAAAAdAAAAABAJ)
## Key Features
- **To-Do Lists**
  
        Ability to create, organize, prioritize, and categorize tasks
- **Calendar Scheduling**
  
        A visual calendar view for daily, weekly, or monthly planning
- **Time Tracking**
  
        A timer to track the time spent on tasks or projects
- **Reminders**

        Customizable notifications and reminders for deadlines and events
- **Collaboration**
  
        Share tasks, projects, or calendars with team members or colleagues

---
## Installation Guide
### For Windows:
 1. Locate the downloaded file (e.g., `FocusProSetup.exe`) in your **Downloads** folder
 2. Double-click the file to start the installation
   
 3. Follow the on-screen instructions, and select:
     - Installation Folder (default is usually fine)
     - Create a Desktop Shortcut (optional)
 4. Click “**Install**” and wait for the installation to complete.
 
 5. Once finished, click “**Finish**” to launch the app

### For macOS
 1. Locate the downloaded file (e.g., `FocusPro.dmg`) in your **Downloads** folder
 
 2. Double-click the file to open the installation window
 
 3. Drag the "**FocusPro**" icon into the Applications folder 
 
 4. Open the Applications folder and double-click "**FocusPro**" to launch the app  

### For linux 
  1. Locate the downloaded file (e.g., `FocusPro.tar.gz` or `FocusPro.deb`) in your **Downloads** folder
   
  2. Open a terminal window
   
  - For `.deb` Package (Ubuntu, Debian[^3]):
     ```bash
     cd ~/Downloads
     sudo dpkg -i FocusPro.deb
     ```
     - If any dependencies are missing, fix them with:
       ```bash
       sudo apt-get install -f
       ```
  
  - For `.tar.gz` Package (General Linux[^3]):
     ```bash
     cd ~/Downloads
     tar -xvzf FocusPro.tar.gz
     cd FocusPro
     ./install.sh
     ```
  
  1. Follow any on-screen instructions provided by the installation script
---   
## User Guide
### Creating a New Project:
- [x] Open Chronos app
- [x] Navigate to “Projects” tab
- [x] Click on “+ New Project” button
- [x] Enter project name
- [x] Set a project deadline
- [x] Add an optional description
- [x] Assign team members(if needed) 
- [x] Create tasks related to the project
- [x] Click “Save” or “Create Project”

### Collaboration

Chronos offers collaboration features to utilize teamwork and communication 

| Collaboration Option     | Description                                      | Benefits                            |
|--------------------------|--------------------------------------------------|-------------------------------------|
| **Shared Projects**      | Projects can be shared among team members.     | Easy access and collaboration.      |
| **Task Assignments**     | Assign specific tasks to individual members.    | Clear accountability for tasks.     |
| **Comments and Feedback**| Team members can leave comments on tasks.       | Facilitates communication and updates. |
| **comunication Chat**       | In-app messaging for instant communication.     | Quick discussions without leaving the app. |

### Reporting

Users can generate reports in Chronos to track project progress, task completion, and overall performance metrics. These reports can be customized based on project needs and can be exported in various formats.

- Generating a Report:
1. Navigate to the **“Reports”** section in the Chronos app.
2. Select the project for which you want to generate a report.
3. Choose the report type (e.g., progress report, completion report).
4. Click **“Generate Report”**.
5. The report will be generated and available for viewing or exporting.

- Example of a Generated Report in JSON Format:

```json
{
  "projectName": "Website Redesign",
  "startDate": "2024-01-15",
  "endDate": "2024-04-30",
  "tasks": [
    {
      "taskName": "Design Mockups",
      "assignedTo": "Alice",
      "status": "Completed",
      "dueDate": "2024-02-10"
    },
    {
      "taskName": "Develop Frontend",
      "assignedTo": "Bob",
      "status": "In Progress",
      "dueDate": "2024-03-15"
    },
    {
      "taskName": "Testing",
      "assignedTo": "Charlie",
      "status": "Pending",
      "dueDate": "2024-04-20"
    }
  ],
  "overallStatus": "In Progress",
  "completionPercentage": 33
}
```
---
## Troubleshooting

Here are some common issues users might encounter while using Chronos

- **Issue: Unable to Create a New Project**
  - ***Definition***:  
    Users may experience difficulties when trying to create a new project, often due to missing required fields or app permissions
  - ***Solution***:  
   Ensure that all required fields (project name, deadline) are filled out correctly. Check that you have the necessary permissions to create projects within the app settings

- **Issue: Syncing Problems with Calendar**
  - ***Definition***:  
   Users may find that their tasks and deadlines are not syncing correctly with their external calendar (e.g., Google Calendar, Outlook)
   - ***Solution***:  
  Verify that your external calendar integration is properly configured in the settings. Try disconnecting and reconnecting your calendar account. If issues persist, check for any app updates

- **Issue: Slow Performance or App Crashes**
   - ***Definition***:  
   Some users might experience lagging, freezing, or crashing while using the app, especially with large projects or many tasks
  - ***Solution***:  
  Ensure that your device meets the app’s minimum system requirements. Close any unnecessary applications running in the background. If the problem continues, try reinstalling the app or clearing the app cache (if applicable)

For further assistance, please refer to the support section or contact customer support[^1].

--- 

## Advanced Usage

### How to Use Scripting in Chronos

1. **Access the Scripting Interface**:
   - Open the Chronos app and navigate to the **"Automation"** section from the main dashboard.
   - Click on the **"Create Script"** button to open the scripting editor.

2. **Write Your Script**:
   - Use the provided syntax to define your automation tasks. The editor typically includes helpful hints and examples.

3. **Test Your Script**:
   - After writing your script, use the **"Test"** button to run it in a controlled environment. This helps ensure there are no errors before applying it to real tasks.

4. **Save and Schedule Your Script**:
   - Once you are satisfied with the script, save it and set a schedule for when you want it to run (e.g., daily, weekly, or on specific events).

5. **Monitor and Adjust**:
   - Regularly check the performance of your automated tasks. Adjust the script as needed to optimize its functionality.

### Example Script

Below is a simple example script that automatically creates a weekly reminder task for a team meeting every Monday at 10 AM[^2].

```java
import java.util.Calendar;

public class ChronosReminder {
    
    public static void main(String[] args) {
        String taskTitle = "Weekly Team Meeting";
        String taskDescription = "Discuss project updates and action items.";
        
        Calendar dueDate = Calendar.getInstance();
        dueDate.set(Calendar.DAY_OF_WEEK, Calendar.MONDAY);
        if (dueDate.getTimeInMillis() < System.currentTimeMillis()) {
            dueDate.add(Calendar.WEEK_OF_YEAR, 1); 
        }
        dueDate.set(Calendar.HOUR_OF_DAY, 10); 
        dueDate.set(Calendar.MINUTE, 0);
        dueDate.set(Calendar.SECOND, 0);
        
        createTask(taskTitle, taskDescription, dueDate.getTime());
    }
    
    public static void createTask(String title, String description, java.util.Date dueDate) {
        System.out.println("Creating task:");
        System.out.println("Title: " + title);
        System.out.println("Description: " + description);
        System.out.println("Due Date: " + dueDate);
        System.out.println("Priority: Medium");
        System.out.println("Tags: meeting, weekly");
        
         new String[]{"meeting", "weekly"});
    }
}
```
### Integrations

| Application Name       | Description                                           | Website                        |
|------------------------|-------------------------------------------------------|--------------------------------|
| **Google Calendar**    | A widely used calendar application for scheduling events and reminders. | [Google Calendar](https://calendar.google.com) |
| **Trello**             | A project management tool that uses boards, lists, and cards to organize tasks. | [Trello](https://trello.com)   |
| **Microsoft Teams**    | A communication platform that integrates chat, video meetings, and file collaboration. | [Microsoft Teams](https://teams.microsoft.com) |
| **GitHub**             | A platform for version control and collaboration for software development projects. | [GitHub](https://github.com)   |
| **Evernote**           | A note-taking app that allows users to organize notes, tasks, and ideas in one place. | [Evernote](https://evernote.com) |


# FOOTNOTES
[^1]:
### to contact us:
S444001990@UQU.EDU.SA

[^2]: 
### another example of creating a weekly reminder task
```javascript
// Script to create a weekly reminder task for team meeting

const taskTitle = "Weekly Team Meeting";
const taskDescription = "Discuss project updates and action items.";
const dueDate = new Date(); // Current date
dueDate.setDate(dueDate.getDate() + (1 + 7 - dueDate.getDay()) % 7); // Next Monday
dueDate.setHours(10, 0, 0); // Set time to 10 AM

// Function to create a new task
function createTask(title, description, dueDate) {
    return Chronos.Tasks.create({
        title: title,
        description: description,
        dueDate: dueDate,
        priority: 'Medium',
        tags: ['meeting', 'weekly']
    });
}

// Schedule the task creation for next Monday
createTask(taskTitle, taskDescription, dueDate);
```
THIS WILL HELP YOU COMPRIHENS THE CODE MORE

[^3]:
### more infos about the difference between **Ubuntu** and **General Linux** 
- Linux is a broad term that encompasses all operating systems built around the Linux kernel.
- Ubuntu is a specific user-friendly Linux distribution derived from Debian, designed to be accessible and widely supported.
In essence, Ubuntu is a Linux distribution, but not all Linux distributions are Ubuntu. Ubuntu takes the Linux kernel and adds its own customizations, software, desktop environment, and tools to create a cohesive operating system.


