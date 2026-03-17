# CSS Architecture Rules — DO NOT VIOLATE

This repository uses a **layered CSS system**.

All agents MUST follow this structure when writing or modifying CSS.

---

# 1. CSS Layer System

There are ONLY two valid CSS layers:

## A. Global CSS (single source of truth)

Location:

```
/css/style.css
```

Contains ONLY:

* layout system
* spacing
* base components

### Allowed global classes:

```
.page
.two-col
.card
.rule-block
.dd
.sys-grid
.ss
```

These classes must be defined **ONCE and only once**.

--- 

### Component Grouping Rule 

All styles belonging to a single component must be grouped together.

Example:
All `.cover-*` classes must exist in a single COVER block inside `/css/style.css`.

Do not scatter component styles across the file.


---

## B. Section CSS (scoped only)

Location:

```
/components/{section}.css
```

Contains ONLY:

* section-specific styles
* unique component classes

---

# 2. Hard Rule — No Base Class Duplication

The following classes MUST NEVER appear outside `/css/style.css`:

```
.page
.two-col
.card
.rule-block
.dd
.sys-grid
```

---

# ❌ INVALID

```css
.page{
padding:40px;
}
```

---

# ✅ VALID

```css
.voice-block{
margin-top:20px;
}
```

---

# 3. Naming Convention (Required)

All section-specific classes must be prefixed:

```
{section}-{element}
```

Examples:

```
voice-rule
voice-note
eco-node
eco-layer
ig-post
```

---

# 4. Conflict Resolution Rule

If a section requires changing a global class:

❌ DO NOT edit the class locally
❌ DO NOT override it inside the component

✅ Instead:

1. Update `/css/style.css`
2. Apply change globally

---

# 5. Responsive Rules

Responsive behavior must follow global patterns:

```
two-col → collapses to 1 column under 768px
grid → collapses to 1 column under 768px
```

Do NOT redefine breakpoints inside components.

---

# 6. Enforcement Rule (Critical)

Before committing CSS:

* Check for duplicate class definitions
* Check for global class overrides
* Check for conflicting layout rules

If any are found:

→ REMOVE them
→ Move logic to `/css/style.css`

---

# 7. Mental Model

Global CSS = system
Component CSS = decoration

If a class affects layout across sections → it is GLOBAL
If a class affects only one section → it is LOCAL

---

Failure to follow these rules will result in:

* layout inconsistencies
* broken responsive behavior
* cascading override conflicts
* agents rewriting unrelated sections

Do not violate this.
