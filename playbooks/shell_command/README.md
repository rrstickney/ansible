# Shell Command Playbook

This playbook is designed to execute shell commands on remote hosts and display their output.

## Usage

1. **Clone the Repository:**

   Clone this repository to your local machine:

   ```bash
   git clone git@github.com:rrstickney/ansible.git
   ```

2. **Navigate to the playbook directory:**

   ```bash
   cd playbooks/shell_command
   ```

3. **Run the playbook:**

   Execute the playbook by providing the shell command as a variable using the `--extra-vars` option:

   ```bash
   ansible-playbook shell_command.yml --extra-vars "shell_command='your_shell_command_here'"
   ```

   Replace `'your_shell_command_here'` with the actual shell command you want to execute.

## Example

Suppose you want to run the `ls -l` command on all hosts. You would execute the following command:

```bash
ansible-playbook shell_command.yml --extra-vars "shell_command='ls -l'"
```

This will execute the `ls -l` command on all hosts and display the output.
