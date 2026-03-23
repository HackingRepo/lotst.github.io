# Contributing to LOTST Awareness Project

Thank you for your interest in contributing! This project documents **Living Off The Security Tools (LOTST)** scenarios for awareness and education. Each page highlights how trusted security platforms could be abused, and how defenders can mitigate risks.

---

## 📐 Style Guidelines

When adding a new tool awareness page:

- **File Naming**
  - Use lowercase, hyphen-separated filenames.
  - Example: `fortinet-fortigate.html`, `elastic-security.html`.

- **Structure**
  - Each file must be a standalone HTML page.
  - Sections:
    1. **Header**: Project title and tool name.
    2. **Warning Banner**: Clear disclaimer that content is for awareness only.
    3. **Concept**: Short description of the tool and its legitimate purpose.
    4. **How Abuse Could Look**: Bullet list of potential abuse scenarios.
    5. **Defensive Takeaways**: Bullet list of defensive recommendations.
    6. **Footer**: Project disclaimer.

- **Visual Style**
  - Use a **color theme** that reflects the tool’s branding (e.g., blue for Microsoft, red for Fortinet).
  - Rounded corners, subtle shadows, and clean typography.
  - Consistent layout across all pages.

- **Tone**
  - Professional, educational, and neutral.
  - Never provide attack instructions.
  - Always emphasize defensive awareness.

---

## 🛠️ Adding a New Tool

1. **Create a new HTML file** in the project root.
2. **Follow the template**:
   - Update the `<title>` and header text with the tool name.
   - Adjust the theme color in CSS to match the tool’s branding.
   - Fill in the **Concept**, **Abuse Scenario**, and **Defensive Takeaways** sections.
3. **Test locally** to ensure consistent styling and readability.
4. **Add a link** to the central `index.html` navigation so visitors can access the new page.

---

## ✅ Example Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>LOTST Awareness - [Tool Name]</title>
  <style>
    /* Update theme color */
    header, h2, footer { background: [brand-color]; color: #fff; }
    /* Keep consistent layout */
  </style>
</head>
<body>
  <header>
    <h1>Living Off The Security Tools (LOTST)</h1>
    <p>Awareness for [Tool Name] and similar platforms</p>
  </header>

  <section>
    <div class="warning">⚠️ Awareness only. No attack instructions.</div>
    <h2>Concept</h2>
    <p>[Describe tool’s legitimate purpose]</p>
  </section>

  <section>
    <h2>How Abuse Could Look</h2>
    <ul>
      <li>[Abuse scenario 1]</li>
      <li>[Abuse scenario 2]</li>
    </ul>
  </section>

  <section>
    <h2>Defensive Takeaways</h2>
    <ul>
      <li>[Defense 1]</li>
      <li>[Defense 2]</li>
    </ul>
  </section>

  <footer>
    <p>LOTST Awareness Project - Educational Use Only</p>
  </footer>
</body>
</html>
```

By following that, We take contribution seriously for that repo, We appreciate PRs that follow our contributions guidelines and comply with the License **GPL 3.0** for adding new security tools, For orgs to protect themselv against LOTST.
