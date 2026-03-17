# 05

Final Section Name: LOGO USAGE
Layout Source Reference: style_guide_12.html
Style Reference: style_guide_12.html
screenshot layout reference: image%2010.png
LAYOUT CODE REF: <div class="lp-nav">

<div class="lp-nav-brand">
Wine Wankers
</div>

<div class="lp-nav-links">
<a class="lp-nav-link">Events</a>
<a class="lp-nav-link">Wine</a>
<a class="lp-nav-link">About</a>
</div>

</div>
SECTION COPY - COMPLETE: 05. Logo Usage
Logo Treatment
Always use the PNG asset
logo.png is the primary logo. Use it in the hero. Never replace with styled text, CSS-generated text, or icon systems. Must feel familiar to Nick.

Hero placement
Centered. max-width:560px. width:100%. Below the positioning kicker, above the hero title. Dominant and memorable — the emotional anchor of the hero.

Logo colour #e040a0 in context
Wine Wankers

Nav brand mark
Wine Wankers

Footer text mark
#e040a0 — logo, nav brand, footer mark only. ALWAYS in Crushky for nav/footer where logo.png is missing. Not dominant fill.
Correct
PNG logo in hero, full size, centered. Logo pink (#e040a0) as text mark in nav and footer where logo would be too large.

Incorrect
Scaling below recognisable size. Adding glow or drop-shadow effects to the logo. Omitting from hero.
STYLE CODE REF: HTML: 
<div class="lp-nav">

<div class="lp-nav-brand">
Wine Wankers
</div>

<div class="lp-nav-links">
<a class="lp-nav-link">Events</a>
<a class="lp-nav-link">Wine</a>
<a class="lp-nav-link">About</a>
</div>

</div>
css: .lp-nav-brand{
font-family:'Crushky','Instrument Serif',Georgia,serif;
font-style:italic;
font-size:20px;
color:var(--pink);
}
screenshot style reference: image%2011.png