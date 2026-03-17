# Component Rules

Components must follow these rules.

1. Components contain **only section HTML**.
2. No `<style>` blocks allowed inside components.
3. No `<script>` tags.
4. Components must use existing global classes.
5. Components must not contain inline styles.

All styling must be defined in /css/style.css.


Example:

```
<section id="section-02" class="page">
```

NOT:

```
<html>
<head>
<style>
```

---

# CSS Policy

All CSS must live in:

```
/css/style.css
```

Agents must not redefine:

.page
.two-col
.card
.rule-block
.sys-grid
