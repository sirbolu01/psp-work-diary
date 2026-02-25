# Week 6

## Week 4 Progress Update – MollyLimpets (Group 3)

Consideration of Software, Hardware and Preparations for a Successful Sprint
During Week 4, our focus shifted towards ensuring that all technical and practical preparations were in place to support a successful sprint. Having experienced configuration and integration challenges in earlier weeks, we recognised that preparation is just as important as implementation.
To deliver the client’s requirement — a simple database-driven system capable of searching garments by chest and waist size and displaying stock quantities and location — we needed a stable and consistent development environment across the team.

1. Software Preparation
A successful sprint depends heavily on correct software setup. For our project, this included:
Backend Environment
•	.NET 6 SDK installed and updated
•	Visual Studio configured correctly
•	Verified appsettings.json configuration
•	Confirmed correct API port and routing
Database Environment
•	MySQL Server running locally
•	MySQL Workbench installed
•	Database schema correctly initialised using setup script
•	Database user permissions configured
•	Connection string verified and tested
Frontend Environment
•	Node.js installed (correct version)
•	Dependencies installed via npm install
•	API base URL correctly configured
•	Frontend development server tested
Version Control
•	Git installed and configured
•	GitHub repository accessible
•	Branching strategy agreed
•	Pull request workflow confirmed
•	.gitignore configured correctly
Ensuring all team members had identical or compatible software versions reduced integration inconsistencies.

2. Hardware Preparation
Although the project does not require specialised hardware, several considerations were still important:
•	Laptops capable of running backend server and frontend concurrently
•	Sufficient RAM to run MySQL, Visual Studio, and Node.js simultaneously
•	Stable internet connection for GitHub synchronisation
•	Access to university labs as backup in case of personal device issues
We also ensured regular backups via GitHub to prevent data loss.

3. Configuration and Environment Consistency
One of the most important lessons from previous weeks was the impact of configuration mismatches. Therefore, Week 4 emphasised:
•	Double-checking port numbers
•	Confirming API endpoints match frontend calls
•	Verifying database credentials
•	Testing local setup before beginning sprint tasks
•	Documenting setup steps clearly in the README
This preparation reduced time lost to troubleshooting during development.

4. Task and Sprint Planning Preparation
Beyond technical setup, we also prepared organisationally:
•	Reviewed Sprint objectives
•	Reconfirmed client priorities (simple garment search, stock count, location display)
•	Broke down tasks into backend, frontend, and testing components
•	Defined “done” criteria for each feature
•	Assigned responsibilities clearly
We also agreed that no new features would be introduced unless the core search functionality remained stable.

5. Risk Preparation and Mitigation
We identified potential sprint risks:
•	API integration failures
•	Database query errors
•	Merge conflicts in GitHub
•	Time constraints
To mitigate these:
•	Backend endpoints would be tested independently before frontend integration
•	Smaller commits would be made more frequently
•	Pull requests would be reviewed before merging
•	Integration testing would occur mid-sprint, not only at the end

Reflection
Week 4 reinforced that successful software development is not just about writing code, but about preparation, environment stability, and coordination.
Earlier in the project, we experienced configuration issues that slowed progress. This week, we proactively focused on preventing similar problems by standardising software versions, verifying database access, and clearly documenting setup steps.
I have learned that:
•	A sprint can fail before it begins if preparation is weak.
•	Environment consistency reduces integration delays.
•	Clear documentation supports team efficiency.
•	Preparation directly impacts productivity and confidence.
Moving forward, I will continue prioritising structured setup and validation before beginning development tasks. Establishing stable foundations ensures that we can focus on delivering reliable functionality that meets the client’s requirement for accurate garment search, stock visibility, and location tracking.

