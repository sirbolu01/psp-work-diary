# Week 7 Report: Implementation, Integration, and Debugging of the System
## Objective for Week 7

During Week 7, the team continued implementing the Action Plan developed after Sprint One, focusing on refining both frontend and backend functionality. A key part of this week involved setting up and running the full system locally, which highlighted several integration and configuration challenges that needed to be resolved.

## Frontend Progress
The frontend (built using SvelteKit) was successfully run using the development server. This confirmed that the project structure and dependencies were correctly configured.
User interface refinements were made to support the core requirement of searching garments by chest and waist size. Improvements included:
Ensuring input fields are clear and intuitive
Structuring results to display stock count and location clearly
Providing feedback when no results are found

These changes ensured the frontend remained aligned with the client’s requirement for simplicity and usability.

## Backend Setup and Execution
This week marked the first successful attempt to run the backend API locally using the .NET environment.
The backend project was identified as an ASP.NET application and executed using the dotnet run command.
Several warnings were identified during execution, including outdated framework usage and package vulnerabilities. While these did not prevent execution, they highlighted areas for potential future improvement.
## Debugging and Issue Resolution
A critical issue occurred when attempting to start the backend. The application failed due to a missing directory error, caused by a hardcoded file path referencing a different system environment.
The error indicated the backend was attempting to access a directory on a local drive that did not exist on the current machine.

Resolution steps:

Identified and adjusted the incorrect file path.
Reconfigured the application to use a valid local directory.
Created the required folder (wwwroot) to ensure compatibility.

After these fixes, the backend was able to run successfully.

## Frontend–Backend Integration
Verified that API endpoints could be accessed locally.
Ensured the frontend sends correct requests to the backend.
Checked that returned data (stock and location) is displayed accurately.

This step was essential in validating that the system works as a complete application, rather than separate components.

## Testing and Validation
Testing focused on end-to-end functionality:
Running both frontend and backend simultaneously
Testing search functionality through the user interface
Verifying results against expected database outputs

This confirmed that the system is moving closer to meeting the client’s core requirements.

Alignment with the Action Plan
Focused on refining existing functionality rather than adding new features.
Improved reliability through debugging and testing.
Ensured a simple and functional user experience.

The debugging process reinforced the importance of consistent configurations across environments.

Personal Reflection
Week 7 provided valuable experience in troubleshooting and system integration.
Resolving initial backend setup issues improved understanding of how environment configuration impacts application behavior.

## Key lessons learned:

Small configuration issues (such as incorrect file paths) can prevent an entire system from running.
Debugging is a critical part of development, not just an obstacle.
Running a full-stack application requires coordination between multiple technologies.
Testing must include real execution, not just code review.

Next steps:

Ensure configurations are environment-independent.
Test frontend and backend components together regularly to avoid similar issues.
## Deployment & Documentation Considerations
Fixed backend configuration issues caused by hardcoded paths.
Created the missing wwwroot folder to ensure the backend runs locally.
Verified that frontend and backend communicate correctly with valid endpoints.
Documented the setup process to ensure team members can run the system on their own machines.