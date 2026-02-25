# Week 6

## Development of an Action Plan Following Sprint One
Following the completion of Sprint One, our team developed a structured Action Plan to guide Sprint Two and subsequent development. Sprint One successfully established backend connectivity, API functionality, and frontend–backend integration. However, client feedback clarified that the primary goal is not technical complexity but a simple, reliable database program that allows users to:
•	Search garments by specific chest and waist size
•	View how many matching garments are in stock
•	Identify the physical storage location of those garments
This feedback significantly shaped our Action Plan.

Reflection on Sprint One
Sprint One focused primarily on technical foundations:
•	Database setup and schema validation
•	API endpoint creation
•	Frontend–backend communication
•	Environment configuration
While these were necessary, we recognised that the client’s priority is usability and clarity of the garment search function. Therefore, our Action Plan shifts from infrastructure-focused work to requirement-focused refinement.

The Team’s Action Plan
1. Refine Core Search Functionality (Priority 1)
The first objective is to ensure the garment search function works flawlessly.
Actions:
•	Review SQL queries filtering by chest and waist size.
•	Validate that stock count calculations are accurate.
•	Confirm that location data is consistently returned.
•	Test multiple size combinations to ensure reliability.
•	Optimise query efficiency where necessary.
Definition of Done:
•	Search returns correct results for all valid size combinations.
•	Stock quantity matches database records.
•	Location information is clearly displayed.

2. Simplify and Improve User Experience
Because the client emphasised simplicity, we will:
•	Ensure search inputs are clear and intuitive.
•	Improve error handling (e.g., no results found).
•	Display results in a structured, readable format.
•	Remove unnecessary interface complexity.
The focus is clarity over aesthetic complexity.

3. Strengthen Backend Validation
To ensure long-term stability:
•	Add validation for invalid size inputs.
•	Implement error handling for failed database queries.
•	Improve API response consistency.
•	Standardise response formats.
This reduces risk and improves maintainability.

4. Improve Documentation and Configuration Clarity
Based on earlier integration challenges, our Action Plan includes:
•	Standardising configuration setup instructions.
•	Confirming consistent API base URLs.
•	Documenting environment setup clearly in README.
•	Ensuring all team members use the same configuration structure.
This supports smoother collaboration in future sprints.

5. Structured Testing Approach
We recognised that testing must become more deliberate.
Actions:
•	Independent backend endpoint testing before frontend integration.
•	Regression testing after every major change.
•	Peer testing within the team.
•	Verification against client requirement checklist.
Testing will focus specifically on:
•	Accuracy of size-based search
•	Correct stock counts
•	Correct location display

Alignment with Client Requirement
The key development in our thinking after Sprint One is that the system must not become unnecessarily complex. The client clearly wants a straightforward database program, not an enterprise-level inventory management system.
Therefore, our Action Plan prioritises:
•	Reliability over new features
•	Simplicity over architectural sophistication
•	Accuracy over visual enhancements
•	Team alignment over individual preference
Every planned improvement is now measured against one core question:
Does this help the user quickly search by chest and waist size and clearly see stock and location?
If the answer is no, it is deprioritised.

Personal Reflection
Developing the Action Plan helped me understand the importance of iterative refinement in Agile development. Sprint One was foundational, but Sprint Two must deliver visible value aligned directly with client needs.
I also learned that:
•	Client clarification should reshape technical priorities.
•	Simplicity is a design decision, not a limitation.
•	A sprint review should lead to concrete adjustments.
•	Clear action steps prevent repeating earlier mistakes.
Going forward, I will focus on ensuring that development decisions remain aligned with the agreed Action Plan and the client’s emphasis on a simple, accurate garment search system.

