# Wine Wankers — Style Guide Build Repository

This repository reconstructs the **final Wine Wankers Brand Style Guide** from multiple historical HTML versions.

The final output is:

```
/master/style_guide_FINAL.html
```

---

# Project Goal

Create a **clean, production-ready HTML style guide** by combining the correct sections from previous versions.

The repository exists to:

* reduce AI context size
* isolate UI components
* prevent accidental code corruption
* allow agents to work on one section at a time

---

# Source of Truth

This project operates on a dual-source system:

### 1. Strategic Source (Notion)
Primary planning, roadmap, and decision layer:

→ https://traveling-calculator-d0b.notion.site/32591b204252808a9685cebfab20d20c

FILE REPO VERSIONS:
/docs/notion/source-of-truth/
    		/source_of_truth_md   <-COMPLETE INDIVIDUAL SECTION CONTENT
		/source_of_truth_png  <-STYLE AND LAYOUT SCREENSHOTS
		 source_of_truth.csv  <-RAW CSV DATA
			


### 2. Execution Source (Repository)
All implementation, structure, and UI system logic lives in this repository.

---

## Rule

Notion defines:
→ what to build  
→ priorities  
→ context  

Repository defines:
→ how it is built  
→ final implementation  
→ system structure  

If conflict occurs, **repository implementation takes precedence**.

---

# Repository Structure

```
master/
    style_guide_FINAL.html

components/
    cover.html
    strategic_rationale.html
    

assets/
    logo.png
    crushky.ttf

css/
    style.css

css_reference/
    wine_wankers_landing_FINAL.html

source/
    style_guide/
        v10.html
        v11.html
        v11_patched.html
        v12.html

docs/
    section_map.md
    completion_checklist.md
    agent_workflow.md
    css_architecture_rules.md
    component_rules.md
	notion/
	source_of_truth.html
    	source_of_truth.csv
```

---

# Execution Order (for AI agents)

Agents must follow this sequence.

### Step 1 — Read Documentation

Read:

```
/docs/section_map.md
/docs/completion_checklist.md
/docs/css_architecture_rules.md
/docs/agent_workflow.md
/docs/component_rules.md
```
### Step 1.5 — Load Strategic Context (Notion)

Reference:

→ Notion dashboard (primary strategy layer)  
→ /docs/notion/source_of_truth.html (local fallback)

Use this for:
- priorities
- intent
- section purpose

Do NOT use Notion for layout or CSS decisions.

---
### Step 2 — Build Global CSS

Extract layout framework from:

```
/css_reference/wine_wankers_landing_FINAL.html
```

Create or update the global stylesheet:

/css/style.css

If the file already exists:
→ extend it
→ do not duplicate existing rules
→ do not overwrite unrelated sections
```

Only extract:

* layout containers
* spacing rules
* responsive grid system

Do NOT extract decorative animations.

---

### Step 3 — Build Components

Each section has a fixed output file.

Agents must use the exact mapping below:

/components/cover.html	
	   /strategic_rationale.html  
	   /brand_positioning.html  
	   /colour_hierarchy.html  
	   /typography.html  
	   /logo_usage.html  
	   /design_signatures.html  
	   /social_presence.html  
	   /voice_messaging.html  
	   /brand_ecosystem.html  
	   /community_engine.html  
```
For each section:

1. Open the layout source version.
2. Extract the structural layout.
3. Apply styling from the style source version.
4. Write to the exact corresponding file above.

---

## Rules

- Do NOT create new component filenames  
- Do NOT rename files  
- Do NOT choose a “closest match”  
- Each section maps to exactly one file  

---

Each component must contain **only the section HTML**.

No `<head>`, `<body>`, or `<style>` tags.
No inline styles.
---

### Step 4 — Assemble Final Document

Insert components into:

```
/master/style_guide_FINAL.html
```

in the order defined in `section_map.md`.

---

### Step 5 — QA Audit

Verify:

* section order correct
* responsive layout intact
* no duplicated CSS
* assets load correctly
* fonts load correctly

---

# Important Rules

Agents must:

* modify **only one component at a time**
* never rewrite the entire document
* never move section order
* never duplicate CSS definitions
