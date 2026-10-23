# Activity-Investigating-Data-Persistence
This project is for school purposes only.  IT 126

1. What happened to the task titles when you added them to the list?

The task titles were added to the list and displayed on the screen. The application also showed the total number of tasks.

2. Why could the application display the tasks while it was running?

The tasks were stored in a Dart list in the application's memory. Flutter displayed the tasks while the application was running.

3. What happened after the application process ended and was relaunched?

The previously added tasks disappeared when the application was reloaded. The list became empty because the tasks were stored only in memory and were not saved permanently.

4. Would keeping the list inside a StatefulWidget automatically make the tasks persistent? Explain your answer.

No. A StatefulWidget allows the application to update its screen when data changes, but it does not automatically save data permanently. The tasks can still disappear when the application is restarted.

5. What would the application need to do to preserve the tasks between sessions?

The application needs to save the tasks in persistent storage, such as an SQLite database, and retrieve them when the application is opened again.

6. If the application eventually stored hundreds or thousands of tasks, what problems might arise from managing all the data manually in memory?

Managing many tasks could become difficult because searching, updating, and deleting records would require more work. The data could also be lost when the application closes if it is not saved.

7. How could separating the operations that save and retrieve tasks from the UI make the application easier to maintain?

A repository can handle saving, retrieving, updating, and deleting tasks separately from the user interface. This makes the code more organized and easier to understand, test, and maintain.
