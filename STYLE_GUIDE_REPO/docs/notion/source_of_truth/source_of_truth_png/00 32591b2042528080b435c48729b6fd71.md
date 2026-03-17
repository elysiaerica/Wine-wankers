# 00

Final Section Name: COVER PAGE
Layout Source Reference: style_guide_v11.html
Style Reference: style_guide_v11_patched.html
screenshot layout reference: image.png
Required Edits: Rainbow stack on ‘SPECTRUM’ + add rainbow bar motif in bottom left corner - keep ‘WINE WANKERS’ in crushky brush pink
LAYOUT CODE REF: <section id="section-00" class="cover">

<div class="cover-prism"></div>

<div class="cover-bars">
<div class="rm-bar r"></div>
<div class="rm-bar o"></div>
<div class="rm-bar y"></div>
<div class="rm-bar g"></div>
<div class="rm-bar t"></div>
<div class="rm-bar b"></div>
<div class="rm-bar v"></div>
</div>

<div class="cover-inner">

<div class="cover-tag">
Brand Direction
</div>

<!-- LOGO -->
<div class="cover-logo">
<!-- logo.png goes here -->
</div>

<!-- SPECTRUM TITLE -->
<div class="cover-spectrum-word">
Spectrum
</div>


<!-- SUBTEXT -->
<p class="cover-sub">
The anti-pretentious pour club
</p>

<!-- META -->
<div class="cover-meta">

<div>
<div class="cm-label">Version</div>
<div class="cm-val">FINAL · March 2026</div>
</div>

<div>
<div class="cm-label">Producer</div>
<div class="cm-val">Coupe Co</div>
</div>

<div>
<div class="cm-label">Status</div>
<div class="cm-val">Production-ready</div>
</div>

</div>

</div>

</section>
SECTION COPY - COMPLETE: Brand Direction
WINE WANKERS
Spectrum
The anti-pretentious pour club — visual & verbal system
Version FINAL · March 2026
Producer Coupe Co
.Status Production-ready
STYLE CODE REF: .cover{
min-height:88vh;
display:flex;
flex-direction:column;
justify-content:flex-end;
padding:clamp(60px,10vw,100px) clamp(24px,4vw,60px);
position:relative;
overflow:hidden;
}

.cover-prism{
position:absolute;
top:0;
right:0;
width:60%;
height:100%;
z-index:0;
}

.prism-glow{ /* main gradient / }
.prism-glow-hot{ / highlight layer / }
.prism-wine{ / base tone */ }

.cover-inner{
position:relative;
z-index:1;
max-width:820px;
}

.cover-bars{
position:absolute;
bottom:clamp(28px,4vw,48px);
left:clamp(24px,4vw,60px);
display:flex;
flex-direction:column;
gap:4px;
}

.cover-spectrum-word{
font-size:clamp(56px,9vw,120px);
line-height:.88;
}
css: <section id="section-00" class="cover">

<div class="cover-prism" aria-hidden="true">
<div class="prism-glow"></div>
<div class="prism-glow-hot"></div>
<div class="prism-wine"></div>
</div>

<div class="cover-motif" aria-hidden="true">
<div class="rm-bar r"></div>
<div class="rm-bar o"></div>
<div class="rm-bar y"></div>
<div class="rm-bar g"></div>
<div class="rm-bar t"></div>
<div class="rm-bar b"></div>
<div class="rm-bar v"></div>
</div>

<div class="cover-inner">

<div class="cover-tag-row">
<span class="cover-tag-line"></span>
<div class="cover-tag">Brand Direction</div>
<span class="cover-tag-line"></span>
</div>

<div class="cover-brand-name">Wine Wankers</div>

<h1 class="cover-spectrum-word rainbow-stack">Spectrum</h1>

<h2 class="cover-sub">The anti-pretentious pour club</h2>

<div class="cover-meta">
<div class="cover-meta-item">
<div class="cm-label">Version</div>
<div class="cm-val">FINAL · March 2026</div>
</div>

<div class="cover-meta-item">
<div class="cm-label">Producer</div>
<div class="cm-val">Coupe Co</div>
</div>

<div class="cover-meta-item">
<div class="cm-label">Status</div>
<div class="cm-val">Production-ready</div>
</div>
</div>

<div class="cover-scribble" aria-hidden="true">wine</div>

</div>

</section>
screenshot style reference: image%201.png