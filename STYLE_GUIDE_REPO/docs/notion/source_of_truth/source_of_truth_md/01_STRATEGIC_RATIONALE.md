# 01

Final Section Name: STRATEGIC RATIONALE
Layout Source Reference: style_guide_v10.html
Style Reference: style_guide_v10.html
screenshot layout reference: image%202.png
LAYOUT CODE REF: <section id="section-01" class="page">

<div class="page-label">
<span class="n">01</span> Strategic Rationale
</div>

<h2>Why Spectrum Won</h2>

<p class="page-intro">
Three viable territories were evaluated...
</p>

<div class="territory-grid">

<div class="territory-card">
<div class="territory-badge">Rejected</div>
<h4>Suits, Hipsters, Everyone</h4>
<p>Eclectic, inclusive...</p>
</div>

<div class="territory-card selected">
<div class="territory-badge">Selected</div>
<h4>The Rainbow Direction</h4>
<p>Makes Nick's identity ownable...</p>
</div>

<div class="territory-card">
<div class="territory-badge">Rejected</div>
<h4>Natty Wine Eclectic</h4>
<p>Hand-drawn aesthetic...</p>
</div>

</div>

</section>
SECTION COPY - COMPLETE: 01. Strategic RationaleWhy Spectrum Won
Territory A — Rejected
Suits, Hipsters, Everyone
Eclectic, inclusive, broad direction. Strong execution risk — without a visual signature, the brand reads as another generic wine subscription. No ownable territory, no community signal.

Territory B — Selected ✓
The Rainbow Direction
Makes Nick's existing rainbow identity ownable and intelligent. Executed as optical science — refraction bars, prismatic light, chromatic displacement on "weird". The spectrum reads as pride, science, and counterculture simultaneously without being literal. This is the brand.

Territory C — Rejected
Natty Wine Eclectic
Hand-drawn, lo-fi, zine aesthetic. Better suited for Chasing Rainbows Wine Co. as a standalone retail brand. Lacks the visual authority and scalability needed for Wine Wankers as a community platform.

Why Spectrum Works
The Spectrum direction transforms a rainbow — already part of Nick's existing visual language — into an optical phenomenon. Refraction bars as the brand signature. Chromatic displacement on "weird" as the hero typographic effect. Dark backgrounds as the premium canvas. The system reads as a distinct, ownable visual identity that no competitor in the natural wine space has claimed.
STYLE CODE REF: <section id="section-01" class="page">

<div class="page-label">
<span class="n">01</span> Strategic Rationale
</div>

<h2>Why Spectrum Won</h2>

<p class="page-intro">
Three viable territories were evaluated...
</p>

<div class="territory-grid">

<div class="territory-card">
<div class="territory-badge">Rejected</div>
<h4>Suits, Hipsters, Everyone</h4>
<p>Eclectic, inclusive...</p>
</div>

<div class="territory-card selected">
<div class="territory-badge">Selected</div>
<h4>The Rainbow Direction</h4>
<p>Makes Nick's identity ownable...</p>
</div>

<div class="territory-card">
<div class="territory-badge">Rejected</div>
<h4>Natty Wine Eclectic</h4>
<p>Hand-drawn aesthetic...</p>
</div>

</div>

</section>
css: .territory-grid{
display:grid;
grid-template-columns:repeat(3,1fr);
gap:2px;
}

@media(max-width:768px){
.territory-grid{
grid-template-columns:1fr;
}
}

.territory-card{
padding:24px;
}

.territory-card.selected{
outline:2px solid rgba(247,220,111,.14);
}
screenshot style reference: image%203.png