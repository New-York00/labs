# Definition of version control systems and their purpose

The version control system is a system that writes changes to a file or set of files over time andallowing you to return later to a specific version.
Version control systems purpose:
	1. allows you to return files to the state in which they were before the changes
	2. return the project to its original state
	3. see the changes
	4. see who last changed something
	5. see what caused the error (for example, in the code)
	6. see who set the task
	
# Explanation of the benefits and advantages of using version control in a collaborative environment

	1. Tracking changes for team
	Team keeps an extensive history of all activities on a collection of code, that anyone can use.
	2. Collaboration inside of the team
	Team stores all code in a remote repository, they dont use email, charts or other communication channels to send the code.
	They can always pull (or download) the code locally to their computer or push (or send) the code to this repository.
	With version control team can quickly assemble all critical project files and foster actionable communication to improve code quality. 
	Version control system provides a single source of truth, stakeholders from across a DevOps team can collaborate to build innovative solutions
	or track the work of other team members.

# Overview of different types of version control systems (centralized, distributed, etc.)

	1. Centralized Version Control Systems
	You have a single server that stores all versions of files. All developers have access to these files.
	It is easier for administrators to maintain this scheme, since all files are in one place.
	But if the server fails, then work will stop after it is repaired.
	In addition, you must have a permanent backup of files to another server (or other media).
	2. Distributed Version Control Systems
	Git, Mercurial, Bazaar, Darcs.
	Users copy all repository completely.
	Each copy of the repository is a complete backup of all data.
	DVCS can interact with multiple remote repositories, so you can work with different groups of people, applying different approaches at the same time within the same project.
	3. Local Version Control Systems (Optimistic)
	When you do copy of the file on your own PC and named them file name + date + etc..

# Comparison of popular version control systems (Git, Subversion, Mercurial, etc.)

| GIT | Mercurial |
|-----|-----------|
|Git is a little bit of complex than Mercurial|Mercurial is simpler than Git.|
|Git is less secure|Mercurial is more secure|
|Git has a powerful and effective branching model. | Branching in Mercurial doesn't refer the same meaning as in Git.
Branching in Git is better than Branching in Mercurial.
|Git supports the staging area, which is known as the index file.|There is no index or staging area before the commit in Mercurial.|
|The most significant benefit with Git is that it has become an industry-standard, which means more developers are familiar with it.|Mercurial's significant benefit is that it's easy to learn and use, which is useful for less-technical content contributors.|
|Git needs periodic maintenance for repositories.| It does not require any maintenance.|
|It holds Linux heritage|It is python based.|
|Git is slightly slower than Mercurial.| 	It is faster than Git.|
|Git supports the unlimited number of parents.|Mercurial allows only two parents.|
|more advertised (through github or github)|bitbuchet|