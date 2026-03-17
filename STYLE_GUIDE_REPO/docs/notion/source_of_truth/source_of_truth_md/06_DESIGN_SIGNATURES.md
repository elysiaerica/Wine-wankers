# 06

Final Section Name: DESIGN SIGNATURES
Layout Source Reference: style_guide_12.html
Style Reference: style_guide_12.html
screenshot layout reference: image%2012.png
LAYOUT CODE REF: CSS:
.sys-grid{
display:grid;
grid-template-columns:1fr 1fr;
gap:2px;
background:var(--border);
margin-top:20px;
}

.sys-card{
background:var(--card);
padding:24px;
}

.sys-card-label{
font-family:var(--fm);
font-size:9px;
letter-spacing:.15em;
text-transform:uppercase;
color:var(--txt-ghost);
}

.sys-card h4{
font-family:var(--fd);
font-style:italic;
font-size:18px;
color:var(--cream);
}

.sys-card p{
font-family:var(--fb);
font-size:13px;
color:var(--txt-dim);
}
SECTION COPY - COMPLETE: 06. Design SignaturesRules for developers and designers to maintain consistency without prescribing every element. The signature devices do the heavy lifting.

Layout approach
Generous margins (80px desktop, 24px mobile). 8px grid baseline. Maximum content width 1200px. Cards use border-radius: 2px or none. Asymmetric layouts preferred — left-anchored content, right-edge spectrum elements.

Border & line style
Subtle borders at 1px solid rgba(255,255,255,0.07) on dark backgrounds. 1px solid rgba(0,0,0,0.08) on light. No heavy strokes, no drop shadows. Separation through spacing, not boxing.

Texture & grain
Optional noise overlay at 2–4% opacity on dark sections. No gradients except the spectrum gradient itself. The scribble layer (see below) provides texture in dark contexts without disrupting readability.

Motion notes
Subtle fade-in on scroll (400ms). Spectrum bars animate in sequence (stagger 50ms per beam). No bounce, no elastic easing. Motion should feel like light changing, not UI reacting.Signature element — Refraction Bars
7 staggered bars · spectrum order · decreasing width · hero, section transitions, footers

Scribble layer demo
wine
Instrument Serif italic · opacity .035 · 180–220px · dark sections only · not on light pages

Refraction bar & beam placement rules
1. Hero sections — as the prism light-scatter signature element at base or side. 2. Section transitions between dark pages — not between light sections. 3. Special emphasis — footers, covers, closing statements. Do not use as repeating decorative pattern throughout body content.
STYLE CODE REF: CSS:
.sys-grid{
display:grid;
grid-template-columns:1fr 1fr;
gap:2px;
background:var(--border);
margin-top:20px;
}

.sys-card{
background:var(--card);
padding:24px;
}

.sys-card-label{
font-family:var(--fm);
font-size:9px;
letter-spacing:.15em;
text-transform:uppercase;
color:var(--txt-ghost);
}

.sys-card h4{
font-family:var(--fd);
font-style:italic;
font-size:18px;
color:var(--cream);
}

.sys-card p{
font-family:var(--fb);
font-size:13px;
color:var(--txt-dim);
}
css: CSS:
.sys-grid{
display:grid;
grid-template-columns:1fr 1fr;
gap:2px;
background:var(--border);
margin-top:20px;
}

.sys-card{
background:var(--card);
padding:24px;
}

.sys-card-label{
font-family:var(--fm);
font-size:9px;
letter-spacing:.15em;
text-transform:uppercase;
color:var(--txt-ghost);
}

.sys-card h4{
font-family:var(--fd);
font-style:italic;
font-size:18px;
color:var(--cream);
}

.sys-card p{
font-family:var(--fb);
font-size:13px;
color:var(--txt-dim);
}
screenshot style reference: image%2013.png