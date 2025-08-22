Priority

Created a new Priority.java enum (LOW, MEDIUM, HIGH).

Added it as a field in Task.java (@Enumerated(EnumType.STRING) private Priority priority).

Default = MEDIUM.

Deadline

Added LocalDate deadline field in Task.java.

User can set it via <input type="date">.

Created Date

Added LocalDate createdDate = LocalDate.now(); in Task.java.

Automatically stores the day a task is created.

Notes

Added String notes field to Task.java.

Users can type extra details when creating a task.

Attachments (File Uploads)

Added String attachmentPath in Task.java.

Users can upload files (stored in a local uploads/ folder).

Displayed as a "View File" link in the task list.
