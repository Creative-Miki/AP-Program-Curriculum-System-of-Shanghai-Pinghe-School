# Pinghe AP Pathway Atlas

AP CSP Final Project computational artifact built from the original Shanghai Pinghe AP curriculum prototype.

## Project Track

**Track B: The Smart Campus Architect**

Pinghe AP Pathway Atlas helps students compare AP courses, workload intensity, GPA weighting, prerequisites, and career alignment before choosing a four-year pathway.

## V.I.B.E. Framework

### V - Visual & Aesthetic Excellence

- Editorial interface inspired by magazine dashboards.
- Playfair Display headers, restrained whitespace, and high-contrast data panels.
- Responsive layout for classroom demo screens and laptops.

### I - Interactive Data-Driven Design

- Loads `data/courses.json` with 40 local course records.
- JavaScript filters by grade, discipline, intensity, search text, and student intent.
- Canvas visualizations render department mix and workload intensity dynamically.

### B - Boundaries & AI Security

- Includes a simulated **AI Pathway Advisor**.
- Input is sanitized before rendering.
- Prompt-injection patterns are blocked and logged in a Defense Console.
- The advisor only answers from the local JSON dataset and refuses attempts to reveal hidden rules, execute scripts, or override policy.

### E - Execution for Global Impact

Course selection is often driven by rumor, pressure, or unequal access to senior advice. This project uses computing to make academic planning more transparent, measurable, and defensible.

## Run Locally

Because the app fetches a local JSON file, run it through a local web server:

```powershell
cd D:\Pinghe-AP-Curriculum-VIBE
python -m http.server 4173
```

Then open:

```text
http://localhost:4173
```

## Demo Day Pitch

1. Show the editorial dashboard and explain the student pain point.
2. Filter by grade and discipline to prove local JSON data is driving the UI.
3. Toggle the Canvas visualizations.
4. Build a pathway for an intended major.
5. Ask the AI advisor a normal course-planning question.
6. Run the Injection Demo and explain the defense architecture.

## Suggested GitHub Pages Deployment

```powershell
git remote -v
git checkout -b vibe-final
git add index.html styles.css app.js data/courses.json README.md
git commit -m "Transform curriculum prototype into VIBE AP CSP artifact"
git remote set-url origin https://github.com/YOUR_USERNAME/AP-Program-Curriculum-System-of-Shanghai-Pinghe-School.git
git push -u origin vibe-final
```

Enable GitHub Pages from the repository settings using the branch you publish.
