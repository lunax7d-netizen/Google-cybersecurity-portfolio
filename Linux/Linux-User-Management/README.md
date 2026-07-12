# Linux User Management

## Objective

Learn how to manage user accounts in Linux by creating users, assigning groups, changing file ownership, and removing users using Bash commands.

## Scenario

As part of a cybersecurity lab, I practiced managing user access in a Linux environment. I created a new user account, assigned group memberships, changed file ownership, and removed the user when access was no longer required.

Managing users and permissions is an important responsibility for security analysts to maintain proper authentication and access control.

## Tools Used

- Linux
- Bash
- sudo
- useradd
- usermod
- userdel
- chown

## Commands Used

### Create a New User

```bash
sudo useradd researcher9
```

### Add User to Primary Group

```bash
sudo usermod -g research_team researcher9
```

### Change File Ownership

```bash
sudo chown researcher9 /home/researcher2/projects/project_r.txt
```

### Add User to Secondary Group

```bash
sudo usermod -a -G sales_team researcher9
```

### Delete User

```bash
sudo userdel researcher9
```

### Remove User Group

```bash
sudo groupdel researcher9
```

## Skills Demonstrated

- Linux User Administration
- Authentication Management
- Group Management
- File Ownership Control
- Access Management
- Privilege Management

## Key Takeaways

- Used `useradd` to create new Linux user accounts.
- Used `usermod` to assign primary and secondary groups.
- Used `chown` to change file ownership.
- Used `userdel` to remove user accounts.
- Applied `sudo` for administrative commands.

## Outcome

Successfully managed Linux user accounts by creating users, assigning permissions and groups, changing ownership, and removing access when no longer required. This lab strengthened my understanding of Linux authentication and access management.
