# Introduction to Open Source
Open source software is a software with source code that anyone can inspect, modify, and enhance. The key principle is freedom to use, modify and distribute the software.

**Key Properties**:
1. Source code availability - The code must be open to public
2. Modification allowed - Users can make changes to the source code to suit their needs
3. Redistribution - Users can freely share copies of the software.

On the contrary, a `closed source` software is that software whose:
1. Source code is proprietary and hidden from the public.
2. Usage restrictions are common (e.g.: cannot redistribute or modify)
3. Examples: Microsoft Windows, Adobe Photoshop, etc.

###### Difference table between OSS and CSS

| Open Source                                 | Closed Source                                   |
| ------------------------------------------- | ----------------------------------------------- |
| Source code is available to everyone        | Source code is hidden from the users.           |
| Modification to the source code is allowed. | Modification is not allowed to the source code. |
| OSS are sometimes free.                     | CSS are never free                              |
| The code can be audited for security.       | The code cannot be audited for security.        |
| Community driven, may require self-help.    | CSS is vendor provided.                         |

#### History of OSS
- 1980s-90s - Open source principle date back to the early days of computing, but the movement gained momentum with Richard Stallman's GNU project (1983) and Linus Torvalds's Linux (1991).
- 1998 - The Open Source Initiative (OSI) was formed to promote open source software.
- Today - Open source is widely used, from operating systems to web browsers (Firefox).

---

## Organizations related to OSS

#### Free Software Foundation of India
- It is a non profit organisation which was started in 2001 to promote the use of free/open source software. 
- It delivers talks and workshops to promote free software.

#### Open Source Initiative
The Open Source Initiative is a non profit organization founded in 1998 to: 
- Promote open-source software.
- Maintain the Open Source Definition
- Approve open-source licenses
- Host the Open Source Directory

#### Open Source Communities
Open source is driven by global communities, where developers, testers, and users collaborate. Examples include: 
1. Linux Foundation:
2. Apache Software Foundation
3. GitHub

---

## OSS Development Process
The process of OSS development is comprehensive, collaborative, and involves multiple stages and stakeholders.

1. **The Idea Stage**
	- It all starts with someone noticing a problem or having an idea for improvement.
	- It can be anything from fixing a bug to adding a new feature.
2. **Planning**
	- Before writing any code, the community needs to agree on:
		  1. What exactly needs to be done?
		  2. Why it's important?
		  3. How it should work?
3. **Building**
	- Here's where the real work happens:
		1. A developer creates a copy (fork) of the project.
		2. They makes changes int their own work area.
		3. They write code following the project's guidelines.
		4. They document their changes so others can understand them.
4. **Testing**
	- Before submissions, developers:
		1. Run tests to check their work.
		2. Get other developers to review their code.
		3. Make sure changes do not break existing functionality.
	- This peer review process catches problems early.
5. **Review**
	- Developers submit their changes through "Pull Request" where:
		1. The community discusses the change.
		2. Code gets refined based on feedback.
		3. Ultimately, maintainers decide what gets accepted.
6. **Merging and Releasing**
	- Once the changes are approved by the maintainers, the new changes are merged with the main production branch.
	- New versions are released with proper documentation describing what the changes were.
7. **Maintenance**
	- The process does not stops here.
	- If users report any issues then the developers have to fix the problem. 
	- New features also keeps getting added.

#### PROs of this process
1. Many eyes catch bugs faster.
2. New features come from diverse contributions
3. Users get exactly what they need because they can contribute directly.

#### CONs of this process
1. Managing so many contributors can be tricky.
2. Coming up with efficient contribution patters is very difficult.
3. Since OSS depends on volunteers contributing in their free time, keeping them motivated in long-term is difficult.

---

## LINCENSES in OSS
Licenses are the backbone of the open-source ecosystem, defining what you can and can't do with the code. 

> Open source licenses are software licenses that allow content to be used, modified, and shared. 
> 1. They facilitate free and open-source software (FOSS) development.
> 2. Intellectual property (IP) rights restrict the modification and sharing of creative works.
> These licenses grant the recipient the rights to use the software, examine the source code, modify it and distribute the modifications.

#### Why are they needed?
Open-source licenses create legal frameworks around usage, modification, and distribution of code. They are rulebooks that:
1. Protect original creators
2. Ensure freedom for users
3. Define how the code can be shared or adapted

#### Different types of Licenses

###### Permissive Licenses
These licenses let you basically do anything with the code, with minimal restrictions.

**What users can do?**
1. Use the code for anything.
2. Modify it as you want.
3. Distribute it freely, even in proprietary software.

**What users cannot do?**
1. Alter the original copyright notice.
2. Misinterpreting authorship.
3. Using the project's trademarks or logos in a way that suggests endorsement, unless the license explicitly grants that right.
4. Imposing additional restrictions that are more restrictive than the original ones.

**Examples**:

Lincense:

| License            | Description                                      |
| ------------------ | ------------------------------------------------ |
| MIT License        | Extremely simple and permissive                  |
| Apache License 2.0 | Similar to MIT but with explicit parent grants   |
| BSD Licnenses      | Family of licenses with variations of permission |

Software: `jQuery`, `Ruby on Rails`

###### Copyleft Licenses
All the derivatives must remain open source.

**Two flavours**:
1. **Strong**: Requires all derivates to remain open source. e.g.: GPL
2. **Weak**: Libraries can be used in proprietary software.
   e.g.: LGPL, MPL

**What users are allowed to do?**
1. Users are free to install, run, and execute the software any number of times for personal, academic, or professional purposes.
2. Users are also allowed to modify the source code to meet their needs. 
3. Users are free to distribute copies or even products if they wish to.

**What users are not allowed to do?**
1. They are not allowed to close source the derivatives. 
2. They must not prevent others from seeing the code.
3. They must not remove already existing license and copyrights.
4. They cannot impose additional restrictions on downstream.

