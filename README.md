mock-up-NGS-chatbot
A static, front-end mockup of an internal Staff Assistant chat interface for Newcastle Grammar School. Built to visualise the concept for stakeholders — it is a design prototype, not a working AI tool. Responses are canned and no data leaves the page.
What it is
A single self-contained HTML file emulating an LLM chat interface, styled in NGS branding (navy `#003249`, white base, Poppins). It demonstrates how staff might use a guardrailed assistant to:
Draft parent emails (e.g. a detention notice)
Write Schoolbox posts and announcements
Look up student cohorts by criteria (e.g. Year 12 Economics students)
Reword and tone-check text such as assessment feedback
Features
Centred chat bar with editable suggestion chips beneath it (clicking a chip populates the box so it can be revised before sending)
"Quick help" pop-up modal with additional starting prompts
Animated "liquid" loading indicator while a response is generated
"New chat" button to reset the conversation
Fully responsive; logo and styling embedded so the file works offline
Usage
Open `ngs-staff-assistant.html` in any modern browser. No build step, server, or dependencies required (web fonts load from a CDN when online).
Publishing with GitHub Pages
To host it as a live page:
Rename `ngs-staff-assistant.html` to `index.html`.
In the repository, go to Settings → Pages.
Set the source to your main branch and save.
The site will be served at `https://<your-username>.github.io/mock-up-NGS-chatbot/`.
Status & limitations
Prototype only. All assistant responses are hard-coded demonstrations.
Not connected to any LLM, student information system, or school data.
Sample student names and details are fictional.
The loading animation uses SVG filters, which render best in Chromium-based browsers and Firefox; it degrades gracefully elsewhere.
Next steps (not yet built)
Connect to a real LLM API with an appropriate system prompt and guardrails
Secure, permissioned, read-only access to school systems for genuine cohort queries
Data-governance and privacy review before handling any real student data
