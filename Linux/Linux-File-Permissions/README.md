# Linux File Permissions and Authorization

## Objective

Understand and manage Linux file and directory permissions by examining access controls and modifying permissions to improve system security.

## Scenario

As part of a cybersecurity lab, I analyzed file and directory permissions within a Linux environment. I identified incorrect permissions, removed unauthorized access, and adjusted ownership permissions to protect sensitive files and directories.

Proper authorization controls are essential for preventing unauthorized users from accessing or modifying system resources.

## Tools Used

- Linux
- Bash
- chmod
- ls

## Commands Used

### Navigate to Project Directory

```bash
cd /home/researcher2/projects
```

### View Files and Permissions

```bash
ls -la
```

### Remove Write Permission for Other Users

```bash
chmod o-w project_k.txt
```

### Remove Group Read and Write Permissions

```bash
chmod g-rw project_m.txt
```

### Modify Hidden File Permissions

```bash
chmod ug-w .project_x.txt
```

### Remove Group Execute Permission from Directory

```bash
chmod g-x drafts
```

## Skills Demonstrated

- Linux File Permissions
- Authorization Management
- Access Control
- Bash Command Line Usage
- Security Hardening
- Permission Troubleshooting

## Key Takeaways

- Used `ls -la` to inspect file ownership and permissions.
- Learned how Linux permissions are assigned to users, groups, and others.
- Used `chmod` to modify access permissions.
- Removed unnecessary write and execute permissions.
- Improved system security by restricting unauthorized access.

## Outcome

Successfully analyzed and modified Linux file and directory permissions to enforce proper authorization controls. This lab strengthened my understanding of Linux security practices used by cybersecurity professionals.
