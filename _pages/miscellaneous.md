---
title: "Miscellaneous"
layout: gridlay
sitemap: false
permalink: /miscellaneous/
---

<style>
/* misc page: single-list layout styled like the homepage */
.misc-container{
    max-width: 920px;
    margin: 6px auto 36px auto;
    padding: 6px 12px;
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
    font-size: 1.02rem;
    line-height: 1.55;
    color: #222;
}
.misc-list { list-style: none; margin: 0; padding: 0; }
/* Use CSS grid per row so marker never overlaps content and stays aligned across breakpoints */
.misc-list li {
    display: grid;
    grid-template-columns: 26px 1fr;
    gap: 12px;
    align-items: start;
    padding: 12px 0;
    border-bottom: 1px solid rgba(0,0,0,0.06);
}
.misc-list li::before {
    /* subtle small circular marker that matches site accents; base (neutral) */
    content: '';
    width: 9px;
    height: 9px;
    border-radius: 50%;
    background: rgba(11,92,255,0.32);
    border: 1px solid rgba(11,92,255,0.12);
    justify-self: center;
    align-self: start;
    margin-top: 6px;
    transition: transform .18s ease, background-color .18s ease, box-shadow .18s ease;
}
.misc-list li:last-child { border-bottom: none; }
.misc-list .item-content { max-width: 820px; }
.misc-list a { color: #0b5cff; text-decoration: none; }
.misc-list a:hover { text-decoration: underline; }
.strike-small { color: #666; }
.embed-video { 
    position: relative; 
    padding-bottom: 56.25%; 
    height: 0; 
    overflow: hidden; 
    max-width: 560px; /* narrower for better page balance */
    margin: 10px 0 0 0; /* left-align under the item text */
    border-radius: 6px;
    background: rgba(0,0,0,0.02);
    box-shadow: 0 6px 18px rgba(0,0,0,0.06);
}
.embed-video iframe { 
    position: absolute; 
    top: 0; 
    left: 0; 
    width: 100%; 
    height: 100%; 
    border: 0; 
    display: block;
}


body[data-theme="dark"] .misc-container { color: #e6eefc; }
body[data-theme="dark"] .misc-list li { border-bottom: 1px solid rgba(255,255,255,0.04); }
body[data-theme="dark"] .misc-list li::before { background: rgba(121,168,255,0.18); box-shadow: none; }
body[data-theme="dark"] .misc-list a { color: #9fc7ff; }
body[data-theme="dark"] .strike-small { color: #9aa6b2; }

body:not([data-theme="dark"]) .misc-list li { grid-template-columns: 30px 1fr; border-bottom: 1px solid rgba(0,0,0,0.08); }
body:not([data-theme="dark"]) .misc-list li::before {
    width: 11px;
    height: 11px;
    background: #0b5cff; /* solid brand blue */
    border: 1px solid rgba(11,92,255,0.18);
    box-shadow: 0 8px 20px rgba(11,92,255,0.06);
    margin-top: 4px;
}

/* responsive tweaks */
@media (max-width: 640px) {
    .misc-list li { grid-template-columns: 20px 1fr; gap: 10px; padding: 10px 0; }
    .misc-list li::before { width: 8px; height: 8px; margin-top: 4px; }
}

.misc-list li:hover::before { transform: scale(1.05); background: rgba(11,92,255,0.22); box-shadow: 0 6px 18px rgba(11,92,255,0.06); }

</style>

<div class="misc-container" markdown="1">
<ul class="misc-list">
    <li>
        <div class="item-content"><strike class="strike-small">Sometimes</strike> Rarely, I pen down my musings in my blog. You can find my blog <a href="https://echoesfromanamiablemind.wordpress.com/" target="_blank">here</a>.</div>
    </li>
    <li>
        <div class="item-content">Check out this YouTube video I made with <a href="https://www.kushgrover.com" target="_blank">Kush Grover</a> to introduce Model Checking to school kids:

            <div class="embed-video">
                <iframe src="https://www.youtube.com/embed/4PFSZHYL9Oo" title="Model Checking: An Overview | Kush Grover & Ritam Raha" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
            </div>
        </div>
    </li>
</ul>
</div>
