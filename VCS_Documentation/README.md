# Version Control System (VCS) – Documentation

## Document Details

| Author | Created on | Version | Last updated by | Last edited on |
|------|-----------|---------|----------------|---------------|
| Aditya Raj Singh | 16-01-2026 | Version 1 | Aditya Raj Singh | 19-01-2026 |

---

## Introduction

A Version Control System (VCS) is a tool that helps manage changes to source code and other files over time. It allows multiple users to work on the same project simultaneously while maintaining a complete history of changes.

VCS plays a critical role in modern software development by ensuring code integrity, enabling collaboration, tracking modifications, and supporting rollback to previous versions when needed.

---

## What is a Version Control System (VCS)

A Version Control System is a system that records changes made to files so that specific versions can be recalled later. It helps developers track who made changes, when changes were made, and why those changes were introduced.

---

## Why Version Control System is Used

Version Control Systems are used to:

- Track changes in source code
- Enable collaboration among multiple developers
- Prevent accidental loss of code
- Maintain a history of modifications
- Support parallel development through branching
- Restore previous stable versions when issues occur

---

## Types of Version Control Systems

Version Control Systems can be broadly classified into three types based on how code is stored, accessed, and shared among users.

---

### 1. Local Version Control System (LVCS)

A Local Version Control System manages file versions on a single local machine. In this approach, different versions of files are stored locally, either by manually saving copies or by using simple tools that track changes.

In LVCS, version history is available only on the developer’s system, and there is no built-in mechanism for collaboration with other users. All changes are maintained locally, making it suitable only for individual work.

Local version control systems were commonly used before team-based software development became widespread.

**Example Use Case:**
- Individual developers working on small or experimental projects  
- Manual version tracking using local backups  



### 2. Centralized Version Control System (CVCS)

A Centralized Version Control System uses a single central server that stores the complete repository and version history. Developers connect to this server to check out files, make changes locally, and commit those changes back to the central repository.

The central server acts as the single source of truth, controlling access and maintaining the project history. All version tracking, collaboration, and management are handled through this centralized repository.

**Common Examples:**
- SVN (Subversion)  
- CVS (Concurrent Versions System)  

**Workflow Overview:**
- Developer checks out code from the central repository  
- Makes changes locally  
- Commits changes back to the server  



### 3. Distributed Version Control System (DVCS)

A Distributed Version Control System provides each developer with a complete copy of the repository, including the entire version history. Instead of relying solely on a central server, every user has a full repository locally.

Developers can commit changes locally and later synchronize them with a shared remote repository. This model supports flexible workflows and allows teams to collaborate efficiently across different locations.

**Common Examples:**
- Git  
- Mercurial  

**Workflow Overview:**
- Developer clones the full repository  
- Makes and c

---

## Advantages of Version Control System

- Maintains complete change history
- Enables team collaboration
- Supports branching and merging
- Reduces risk of code loss
- Improves code quality and accountability
- Simplifies release management

---

## Disadvantages of Version Control System

- Initial learning curve for beginners
- Requires proper access control management
- Merge conflicts may occur
- Centralized systems depend heavily on server availability

---

## VCS Workflow


A typical VCS workflow includes:

1. Developer pulls the latest code from the repository  
2. Makes changes locally  
3. Commits changes with a meaningful message  
4. Pushes changes to the repository  
5. Team reviews and merges changes  

---

## Best Practices

- Commit changes frequently with clear messages
- Use meaningful branch names
- Keep the main branch stable
- Review code before merging
- Avoid committing sensitive information
- Regularly pull updates from the repository

---

## Conclusion

A Version Control System is an essential tool in modern software development. It ensures code consistency, enables collaboration, and provides a reliable mechanism to track and manage changes. By following best practices and choosing the right type of VCS, teams can significantly improve development efficiency and software quality.

---

## Contact Information

| Role | Contact |
|----|--------|
| Documentation Owner | tadityaraj.singh18@gmail.com |

---

## References

| Links | Descriptions |
|------|-------------|
| https://git-scm.com/book/en/v2/Getting-Started-About-Version-Control | Official Git documentation explaining Version Control concepts |
| https://www.geeksforgeeks.org/git/version-control-systems/          | Git documentation explaining Version Control concepts|
