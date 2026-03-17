# Wine Wankers Style Guide — Section Map

This document defines the **final section order**, **layout source**, and **style source** for the master document.

---

For strategic context and section intent:
→ see Notion dashboard

---

Agents MUST follow this map when reconstructing sections.

---

## Final Section Order

| ID | Section Name        | Layout Source | Style Source |
| -- | ------------------- | ------------- | ------------ |
| 00 | Cover Page          | v11_patched   | v11          |
| 01 | Strategic Rationale | v10           | v10          |
| 02 | Brand Positioning   | v11           | v11          |
| 03 | Colour Hierarchy    | v10           | v10          |
| 04 | Typography          | v10           | v10          |
| 05 | Logo Usage          | v12           | v12          |
| 06 | Design Signatures   | v12           | v12          |
| 07 | Social Presence     | v10           | v12          |
| 08 | Voice & Messaging   | v11           | v12          |
| 09 | Brand Ecosystem     | v10           | v12          |
| 10 | Community Engine    | v11_patched   | v12          |

---

## Assembly Rules

1. **Section order is fixed.**
2. Layout structure comes from the **layout source version**.
3. Styling and component rules come from the **style source version**.
4. If layout and style conflict:

   * Preserve **layout structure** from layout source.
   * Apply **styling patterns** from style source.
5. Do not invent new sections.

---

## Section Container Pattern

All sections must follow this structure:

```
<section id="section-XX">
    page-label
    section heading
    intro paragraph
    content blocks
</section>
```

Spacing and layout are handled globally via `/css/style.css`.
