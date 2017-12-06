## Highlights

*   Cutting-edge stuff here! So much so we haven't wrote any documentation.

</div>

<div>

## Roadmap

*   Documentation.
*   Performance measurements.

</div>

</div>

## Available Animations

<div class="buttons"><button data-class="-appear-from-bottom">Appear From Bottom</button> <button data-class="-appear-from-left">Appear From Left</button> <button data-class="-appear-from-right">Appear From Right</button> <button data-class="-appear-from-top">Appear From Top</button></div>

<div class="buttons"><button data-class="-blur">Blur</button> <button data-class="-fade-in">Fade In</button> <button data-class="-fade-out">Fade Out</button> <button data-class="-pulsate">Pulsate</button> <button data-class="-wiggle">Wiggle</button></div>

<div class="buttons"><button data-class="-slide-from-bottom">Slide From Bottom</button> <button data-class="-slide-from-left">Slide From Left</button> <button data-class="-slide-from-right">Slide From Right</button> <button data-class="-slide-from-top">Slide From Top</button></div>

</div>

<div class="example -bg-tertiary1">

<div class="flex -pad -text-center -vcenter">

<div>![](http://umbracoflare.com/images/cloudflare-umbraco.jpg)</div>

</div>

</div>

<script>window.app.queue.push(1, 0, function () { var buttons = document.querySelectorAll("[data-class]"), target = document.querySelector("#animate"), lastClass = ""; [].map.call(buttons, function (button) { button.addEventListener("click", function(e){ var value = button.dataset.class; if(lastClass) animate.classList.remove(lastClass); animate.classList.add(value); lastClass = value; }); }); });</script>