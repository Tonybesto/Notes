
### Linux Administration Practice Assignment

#### Objective:
The purpose of this assignment is to enhance your proficiency in Linux command-line administration. You will perform a series of tasks that are common in Linux system management.

#### Tasks:

1. **Basic Command Line Usage**
   - Create a directory structure as follows:
     ```
     /home/student/project/
     ├── src
     ├── bin
     └── docs
     ```
   - Create an empty file named `README.md` in the `docs` directory.
   - Copy the `README.md` file from `docs` to `src`.
   - Move the `README.md` file from `src` to `bin`.

2. **File Permissions and Ownership**
   - In the `project` directory, create a script file named `backup.sh` that contains the following lines:
     ```sh
     #!/bin/bash
     tar -czf /home/student/project/docs_backup.tar.gz /home/student/project/docs
     ```
   - Make the `backup.sh` script executable.
   - Change the ownership of `backup.sh` to the user `student` and the group `student`.
   - Set the permissions of `backup.sh` so that only the owner can execute it.

3. **Process Management**
   - Start a background process that writes the current date and time to a file `/home/student/project/log.txt` every minute. (Hint: You can use the `cron` job or a `while` loop with `sleep` in a script).
   - List all running processes and find the process ID (PID) of the background process you just started.
   - Terminate the background process using its PID.

4. **Disk Usage and Quotas**
   - Check the disk usage of your home directory and save the output to a file named `disk_usage.txt` in the `docs` directory.
   - Set a disk quota of 100MB for the user `student` (Assume you have sudo access for this step).

5. **Networking**
   - Display the IP address of your system.
   - Use `ping` to check connectivity to `www.google.com` and save the first 5 lines of the output to `ping_result.txt` in the `docs` directory.
   - Use `curl` or `wget` to download the homepage of `example.com` and save it as `index.html` in the `docs` directory.

6. **User and Group Management**
   - Create a new user named `testuser` without a home directory.
   - Add `testuser` to a new group named `testgroup`.
   - Change the password of `testuser` to `password123`.

7. **System Monitoring and Performance**
   - Use `top` or `htop` to monitor system performance for 1 minute and note the CPU and memory usage.
   - Save a snapshot of the current running processes to a file named `process_list.txt` in the `docs` directory.

8. **Backup and Restore**
   - Create a compressed archive of the `project` directory and save it as `project_backup.tar.gz` in your home directory.
   - Extract the contents of `project_backup.tar.gz` to a directory named `project_restore` in your home directory.

#### Submission:
- Submit a detailed report with the following:
  - The commands you used for each task.
  - Screenshots showing the successful completion of each task.
  - Any scripts you created.
  - The `project_backup.tar.gz` file.

#### Bonus Task:
- Automate the entire assignment using a Bash script. The script should perform all the tasks mentioned above when executed.

---

This assignment covers various aspects of Linux administration including file management, permissions, process management, disk usage, networking, user management, system monitoring, and backups. By completing these tasks, you will gain hands-on experience and improve your command-line skills.