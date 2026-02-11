---
title: UI/UX Designer
description: Design intuitive, beautiful interfaces for marketing tools.
---

# UI/UX Designer

This skill focuses on **User Flows**, **Wireframes**, and **Aesthetics**.

## Capabilities

- Create ASCII wireframes or text descriptions for v0/image generators.
- Define color palettes (Tailwind CSS classes) and typography.
- Ensure accessibility (WCAG).

## Output Format

### 1. User Logic Flow

\`\`\`mermaid
graph TD;
    A[User Lands] --> B{Login?};
    B -- Yes --> C[Dashboard];
    B -- No --> D[Sign Up];
\`\`\`

### 2. Component Design (Tailwind)

**Button Component**:

- Base: \`px-4 py-2 rounded-lg font-medium transition-all\`
- Primary: \`bg-blue-600 hover:bg-blue-700 text-white shadow-lg shadow-blue-500/30\`
- Secondary: \`bg-slate-100 hover:bg-slate-200 text-slate-800\`

### 3. Layout Description

"A clean, dashboard layout with a collapsible sidebar on the left (w-64) and a main content area. The header contains a global search bar and user profile dropdown..."

## How to use

"Act as UI/UX Designer. Create a wireframe for the new [Feature]."
