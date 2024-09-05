# Jikan - Time Tracking Tool (Readme.md in WIP)

**Jikan** is a powerful time-tracking tool built with C# and WPF (Windows Presentation Foundation). It helps organizations efficiently log and analyze work hours across projects using pre-defined views, customizable graphical reports, and flexible data management options. Jikan supports both SQLite and SQL Server for data storage, making it adaptable to various deployment scenarios.

All the controls, themes, and styles in Jikan are entirely handcrafted, ensuring a unique and customized user experience tailored specifically to the application's needs.

## Features

- **Time Tracking:** Log work hours per project to efficiently track resource usage across the organization.
- **Pre-defined Views:** Analyze logged hours and resource allocation through intuitive, pre-built views that streamline your workflow.
- **Graphical Reports:** Customize data visualizations using pie charts, cartesian charts, and heatmaps. Switch between color schemes and manage report content through filters and groupings.
- **Data Management:** Choose between SQLite and SQL Server for your data storage needs, with the flexibility to add new database support as needed.
- **Settings Management:** Manage essential application settings directly within Jikan.

## Technology Stack

- **Language:** C#
- **UI Framework:** WPF (Windows Presentation Foundation)
- **Database:** SQLite or SQL Server (easily extendable to support additional databases)
- **Additional Libraries:**
  - **Charting Library:** [LiveCharts2](https://github.com/beto-rodriguez/LiveCharts2)
  - **Drag and Drop Support:** [GongSolutions.WPF.DragDrop](https://github.com/punker76/gong-wpf-dragdrop)
  - **Tutorial Overlay:** [GuideLine.WPF](https://github.com/V4SS3UR/GuideLine.WPF)
  - **Toast Notifications:** [ToastManager.WPF](https://github.com/V4SS3UR/ToastManager.WPF)
 
## UI/UX Design

All the controls, themes, and styles in **Jikan** are entirely handcrafted, ensuring a unique and customized user experience. This allows for a cohesive design that is fully tailored to the application's specific functionality and aesthetic.


## Access and Security

### Permissions

  In **Jikan**, managers have enhanced permissions to oversee the time-tracking data of employees who report to them within the organization's flowchart. Through this feature, managers can:    
  - **View Team Data:** Access detailed reports and insights on the work hours logged by their direct reports, allowing for effective monitoring of resource allocation and productivity.      
  - **Log Hours on Behalf of Employees:** If an employee is unavailable to log their own hours, the manager can log the hours on their behalf, ensuring that the team's time-tracking data remains accurate and up-to-date.
  This feature enables managers to maintain oversight of their team’s performance and ensure that all logged hours are correctly recorded.

### Data Visibility

  In **Jikan**, data can be displayed as either the total number of hours worked or as a percentage, providing flexibility in how work is reported. This allows for ethical handling of sensitive information by:
  Here's the paragraph with additional formatting for better readability:
  - **Showing Data as Percentages:** When it’s possible to easily compare the workloads of multiple individuals, the visibility of exact hours is **restricted** to protect employee privacy and prevent unfair comparisons. 
  - **Data as Percentages:** Instead of showing hours, data can be displayed as percentages. This helps maintain confidentiality while still providing insights into overall work distribution.     
  - **Full Data Access:** When workload comparisons are not a concern, all data—including exact hours worked—becomes fully accessible for **in-depth analysis**. 
  This approach ensures ethical data management while still enabling comprehensive resource tracking and analysis.

### Authentication Method

  The current authentication method in **Jikan** is based on retrieving the user's **Windows session email** and **full name**. This approach aligns with my current company's requirements, allowing seamless access without the need for traditional login credentials. By utilizing the user's session information, Jikan ensures a secure and streamlined authentication process.


## Overview

### 1. Register
   Users can quickly register to start tracking their time.
   ![Register](https://github.com/user-attachments/assets/44c7d650-174f-4003-ad42-06a4c5c7b00c)

### 2. Log Work Hours
   Efficiently log and categorize work hours for various projects.
   
   - **Logging Hours:** 
     Track time spent on different tasks and projects, day by day.
     ![HoursReporting](https://github.com/user-attachments/assets/76ad20ff-6c0f-4473-aab4-5b89a59cb11e)

   - **Subject and Favorites Interaction:** 
     Mark tasks or projects as favorites for quicker access, enabling quick import functionality.
     ![HoursReporting_FavoriteSubjects](https://github.com/user-attachments/assets/57cc8c79-c018-4575-8ccb-e3e0229007ab)

   - **Guidelines:** 
     Follow provided guidelines to ensure accurate and consistent time reporting.
     ![HoursReporting_GuideLine](https://github.com/user-attachments/assets/331419be-fdf6-48cf-8c67-d2d8faff5aa4)

### 3. View Reports
   Visualize and analyze the logged data through customizable reports.

   - **User Resource Reports:** 
     View reports focused on individual users or department resources within projects.
     ![Reporting_Users](https://github.com/user-attachments/assets/2bae5514-5ea8-40be-b298-fc051264b328)

   - **Global Resource Reports:** 
     Get an overview of resource allocation across the entire organization. Define custom data for pie charts, cartesian charts, and heatmaps. Use filters to manage what data is displayed and customize the appearance by switching between color schemes.
     ![Reporting_Ressources](https://github.com/user-attachments/assets/563f9ce7-4344-4733-9d59-5fe82cb53ab9)
     
   - **Guidelines:** 
     Follow provided guidelines to ensure accurate usage of the reporting views.
     ![Reporting_Users_GuideLine](https://github.com/user-attachments/assets/ca1092f7-8cc5-4382-b165-b2d0ac76c849)

   - **Time-Based Reports:** 
     Analyze resource utilization over time. Define custom data for charts, and manage filters and appearance settings to suit your needs.
     ![Reporting_Time](https://github.com/user-attachments/assets/c0e75cea-32d1-4ece-bf17-be63817820fa)

### 4. Administration
   Manage your application's settings, data, and organizational structure with ease.

   - **Color Management:** 
     Customize color schemes for each subject.
     ![Settings_Colors](https://github.com/user-attachments/assets/ade88562-6424-40be-ae58-d2066b95abd1)

   - **Database Table Editing:** 
     Modify database tables directly from the application interface.
     ![Settings_EditTable](https://github.com/user-attachments/assets/0b39be46-04b6-4dd8-beb9-5c5aeace2cd3)

   - **CSV Export:** 
     Export data as CSV files for external use or analysis.
     ![Settings_Export](https://github.com/user-attachments/assets/fbd0e3d8-048f-4365-9468-e93bb95b3054)

   - **Missing Data Overview:** 
     Identify and address missing data points for accurate reporting.
     ![Settings_MissingDays](https://github.com/user-attachments/assets/06848f4f-3504-47b6-a099-68eeb6277fb9)

   - **Organization Chart Management:** 
     Visually manage the organization's structure and make adjustments as needed.
     ![Settings_Organization](https://github.com/user-attachments/assets/fd0445a6-36ca-4f99-8f52-c1fc7f9cb54f)
     
   - **Team Management:** 
     Oversee and adjust team configurations for better coordination and reporting.
     ![Settings_TeamManagement](https://github.com/user-attachments/assets/2658ecf7-f54a-4114-ba12-0ba0991017e5)

   - **Server Connection Management:** 
     Set up and manage connections to SQL Server.
     ![Settings_Server](https://github.com/user-attachments/assets/75451888-e207-414d-b40f-889dbc12e2d0)


## Conclusion

Thank you for exploring **Jikan** time-tracking tool designed to streamline project management and resource tracking. As this is a demo project, I welcome your feedback and suggestions on how I can enhance the tool further.

If you have any inquiries, feedback, or just want to share your thoughts, please feel free to contact me.

I hope you find **Jikan** useful and look forward to any comments you might have. Stay tuned for future updates!
