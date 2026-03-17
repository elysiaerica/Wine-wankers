# 09

Final Section Name: BRAND ECOSYSTEM
Layout Source Reference: style_guide_12.html
Style Reference: style_guide_v10.html
screenshot layout reference: image%2018.png
LAYOUT CODE REF: <section id="section-09" class="page">

<div class="page-label">
<span class="n">09</span> Brand Ecosystem
</div>

<h2>Across the ecosystem</h2>

<div class="eco-layout">

<div class="eco-layer">
<div class="eco-layer-label">Primary Brand</div>
<div class="eco-nodes">
<div class="eco-node primary">Wine Wankers</div>
</div>
</div>

<div class="eco-layer">
<div class="eco-layer-label">Online Store</div>
<div class="eco-nodes">
<div class="eco-node">Chasing Rainbows</div>
</div>
</div>

</div>

</section>
SECTION COPY - COMPLETE: 09. Brand Ecosystem
Across the ecosystemHow this direction applies to the three related entities. Each has a distinct treatment — no wholesale adoption, no visual confusion.Primary Brand
Wine Wankers
The full Spectrum direction applies here. Dark backgrounds dominate for event marketing and digital presence. The refraction bars appear as signature elements on posters, ticketing pages, and email headers. Yellow is the primary CTA colour. Instrument Serif headlines, Newsreader body, JetBrains Mono labels. This is the parent brand that could theoretically outgrow any single venue.

Online Store
Chasing Rainbows Wine Co.
A sibling brand sharing the Spectrum DNA but shifting to light mode for e-commerce usability. Aged Paper backgrounds, Wine Stain accents on product cards and category headers. The refraction bars appear as a subtle header strip — the spectrum gradient at reduced opacity, top of page. Typography stays consistent. The name already contains the rainbow — this direction makes that connection explicit and visual.

Host Venue
The End Bar
The End has its own identity and shouldn't adopt Wine Wankers' visual system wholesale. When promoting Wine Wankers events, The End uses a co-branded lockup: their existing aesthetic plus the refraction bars as a "Presented by Wine Wankers" element. Event nights can feature printed spectrum elements that feel additive, not intrusive. Contextual only.

STYLE CODE REF: .eco-layout{
display:grid;
grid-template-columns:1fr 1fr;
gap:24px;
margin-top:20px;
}

@media(max-width:768px){
.eco-layout{
grid-template-columns:1fr;
}
}

.eco-layer{
border:1px solid var(--border);
padding:24px;
border-radius:2px;
}

.eco-layer-label{
font-size:9px;
letter-spacing:.15em;
text-transform:uppercase;
margin-bottom:14px;
display:flex;
align-items:center;
gap:8px;
}

.eco-layer-label::before{
content:'';
width:16px;
height:2px;
display:inline-block;
}

.eco-nodes{
display:flex;
flex-direction:column;
gap:6px;
}

.eco-node{
font-size:13px;
padding:10px 14px;
border-left:2px solid var(--border);
line-height:1.55;
}

.eco-node.primary{
color:var(--cream);
}
css: .eco-layout{
display:grid;
grid-template-columns:1fr 1fr;
gap:24px;
}

.eco-node{
padding:10px 14px;
border-left:2px solid var(--border);
}
screenshot style reference: image%2019.png