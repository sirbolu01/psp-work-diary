# Week 3

# Week 3 Progress Update – MollyLimpets (Group 3)
Comment on the Team’s Approach to Software Development

During Week 3, our team focused on refining how the frontend and backend should be connected and how configuration should be managed across the system. This discussion became important after revisiting the client’s core requirement.

The client specifically stated that they wanted a simple database-driven program where they could:

Search for all garments of a specific chest size and waist size

See how many of those garments are currently in stock

View the physical storage location of those garments

This clarification reinforced that the primary goal of the system is accuracy, reliability, and simplicity — not architectural complexity.

Initially, I suggested using a .env configuration approach for managing frontend–backend communication. My reasoning was that environment-based configuration is scalable, reduces hardcoding, and aligns with industry best practice. It allows flexibility across development and deployment environments.

However, as a team, we discussed whether this level of abstraction was necessary for the current stage of the project. Since the client explicitly wants a simple and reliable database program, we recognised that introducing additional configuration layers might complicate development without adding immediate value.

We therefore agreed that the most important factor is that we are all aligned on a single, consistent method of connecting the frontend to the backend. Even if .env configuration is technically beneficial, simplicity and shared understanding are more important at this stage.

This week helped me understand that:

Software development decisions must align with client requirements.

“Best practice” must be balanced against project scope.

Over-engineering can introduce unnecessary risk.

Team consensus is essential for successful integration.

Ultimately, the system must reliably return garment data filtered by chest and waist size, display accurate stock counts, and show correct location data. Any architectural decision that supports this goal efficiently is appropriate.

How We Will Approach the Sprint Week

To ensure we remain aligned with the client’s requirement for a simple and functional database system, our sprint approach will focus on clarity, structure, and coordination.

1. Requirement-Focused Development

Before starting implementation, we will:

Reconfirm the exact garment search functionality required.

Ensure the database query correctly filters by chest and waist size.

Validate that stock quantity and location fields are returned in the API response.

Keep the solution streamlined and avoid unnecessary complexity.

This ensures that development remains directly aligned with the client’s stated objective.

2. Agreed Frontend–Backend Connection Strategy

To avoid integration issues:

We will agree on a fixed API base URL strategy for the sprint.

Confirm consistent port usage.

Ensure endpoint routes match exactly between frontend and backend.

Document the agreed approach clearly for all team members.

Being on the same page technically is critical to sprint success.

3. Structured Sprint Plan

Planning Phase

Break down tasks into backend, frontend, and testing.

Assign responsibilities clearly.

Define “done” criteria for garment search functionality.

Implementation Phase

Backend: Confirm query accuracy and API response structure.

Frontend: Implement search input and results display.

Validate stock counts and location data visually.

Testing Phase

Test multiple chest/waist combinations.

Confirm accurate stock totals.

Verify correct location mapping.

Perform regression testing to ensure no existing functionality breaks.

Reflection on Personal Development

This week strengthened my understanding that effective software development is not just about implementing technically advanced solutions, but about delivering exactly what the client needs.

While I initially focused on improving configuration structure through .env usage, I realised that alignment with team members and the client’s emphasis on simplicity is more important at this stage.

I am becoming more confident in:

Evaluating when to apply best practice versus when to simplify.

Participating in architectural discussions.

Prioritising client value over technical preference.

Recognising that clarity and consistency reduce integration risk.

Moving forward, my focus will be on ensuring that:

The garment search functionality works flawlessly.

Database queries are efficient and accurate.

Frontend–backend communication is stable.

All team members follow the same technical approach.

Week 3 reinforced that success in full-stack development depends not only on technical knowledge, but also on communication, alignment, and disciplined decision-making.