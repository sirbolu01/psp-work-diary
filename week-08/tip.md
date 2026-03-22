# Week 8 Report: Frontend Enhancement, Security, and Accessibility
## Objective for Week 8

The focus this week was:

Enhance the homepage by adding a Quick Garment Size Check feature for users.
Ensure frontend input validation is robust and user-friendly.
Consider security best practices for running the system publicly.
Consider UI/UX and accessibility issues to improve the overall user experience.
Front-End Contribution (Your Code)

Feature Added: Quick Garment Size Check

Users can input chest and waist measurements and receive immediate feedback.
Validates that the values are numeric and greater than zero.
Provides real-time feedback messages in green (success) or red (error).
Encourages users to proceed to the Garment Search page after validation.

Why it’s your contribution:

You wrote the logic for quickCheck(), including numeric conversion and validation.
You designed the form HTML structure and CSS styling, consistent with the existing menu buttons.
This improves usability and aligns with the client’s requirement for simplicity and clarity.

File Modified: src/routes/index.svelte

Core Code Snippet (your contribution):

<input type="number" bind:value={quickChest} placeholder="Chest size" />
<input type="number" bind:value={quickWaist} placeholder="Waist size" />
<button on:click={quickCheck}>Check Sizes</button>
{#if quickError}
    <p class="{quickError.includes('good') ? 'success' : 'error'}">{quickError}</p>
{/if}

<script>
function quickCheck() {
    quickError = '';
    if (!quickChest || !quickWaist) {
        quickError = "Please enter both chest and waist sizes.";
        return;
    }
    const chestNum = Number(quickChest);
    const waistNum = Number(quickWaist);
    if (isNaN(chestNum) || isNaN(waistNum)) {
        quickError = "Sizes must be numbers.";
        return;
    }
    if (chestNum <= 0 || waistNum <= 0) {
        quickError = "Sizes must be greater than zero.";
        return;
    }
    quickError = `Sizes look good! You can go to Garment Search page to find matches.`;
}
</script>

This snippet is distinctive work for Week 8 because it is client-facing, improves usability, and was implemented entirely by you.

## Security Considerations

Currently, the system runs on HTTP (local http://localhost:3000 or http://192.168.1.112:3000), which is not secure for production.

## Key considerations:

1. Run over HTTPS
Encrypts all communication between client and server.
Prevents attackers from sniffing or tampering with data.
Required for any production deployment handling sensitive information (e.g., customer data).
2. Recommended Deployment for HTTPS
Frontend: Deploy on Vercel or Netlify with automatic HTTPS certificates.
Backend APIs:
Deploy on Azure, AWS, or Vercel Serverless Functions with HTTPS enabled.
Or use a reverse proxy (like Nginx) with HTTPS if self-hosting.
3. Other Security Best Practices
Input validation on both frontend and backend (Quick Check already implemented on frontend).
Avoid storing sensitive data in plain text.
Keep packages updated to patch known vulnerabilities (e.g., System.Data.SqlClient warnings on backend).
Implement CORS policies if frontend and backend are served from different domains.

## UI/UX and Accessibility Considerations
Added clear and intuitive input fields for chest and waist measurements, with placeholders for guidance.
Implemented real-time feedback messages (green for success, red for errors) to provide immediate and understandable results.
Designed the Quick Check form layout to match existing menu button styling, maintaining consistency and visual clarity.
Used appropriate HTML semantics (<input> with type="number", <button>, <p> for messages) to support screen readers and improve accessibility.
Ensured the form is easily navigable with keyboard-only input for accessibility compliance.
Kept font sizes, button sizes, and spacing large enough for readability and usability across devices.