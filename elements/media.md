<div class="breadcrumbs">
[Documentation](/) / Elements / Forms
</div>

# Media

## Highlights

*   Responsive and Non-Responsive Images
*   Image Formats
*   SVG Implementation
*   Video

## Roadmap

*   Animated SVGs
*   Video Formats
*   Figure and captions

## Images

The default behavior of images, within this framework, is that images are never wider than the screen can support. Images will appear at their natural width and height, and scaled down (respecting aspect ratio) when their width is larger than the screen. To make an image fill the entire width of it's own container you can use the class modifier **-block**.

TBD.

<!-- <div class="flex -styleguide">
<div>
A regular image, 300 by 300 pixels:
![Example](https://placeholdit.imgix.net/~text?txtsize=32&bg=dfdfdf&txtclr=ffffff&txt=Example&w=300&h=300&txttrack=0)
</div>
<div>
The same image, with **-block** applied:
![Example](https://placeholdit.imgix.net/~text?txtsize=32&bg=dfdfdf&txtclr=ffffff&txt=Example&w=300&h=300&txttrack=0)</div>
</div> -->

TBD.

## Image Formats

| Format | Name | PROs | CONs |
|--------|------|------|------|
| PNG | Portable Network Graphic | Highest quality images<br>Sharp text<br>Semi-opaque pixels | Largest filesize<br>No animations<br>Grossly overused |
| JPG | Joint Photographic Experts Group | High level of compression allows for "good for the web" quality and low file size<br>Can be downloaded in passes<br>King for photographs | No semi-transparent or transparent pixels<br>No animations |
| GIF | Graphics Interchange Format | Allows for animations<br>Allows for transparent pixels | Limited color pallette<br>No semi-opaque pixels - jagged edges |
| SVG | Scalable Vector Graphics | Will look great at any size<br>Customizeable through CSS<br>Can be animated like GIFs<br>King for icons and branding | Browsers vary widely on implementation<br>Almost certainly requires a JS library to use in the wild |

## SVG

Basic support for the SVG standards is pretty widely adopted by browsers today ([link](http://caniuse.com/#feat=svg)). However, their implementation of the standards are different between the vendors. Working with SVG files moving forward is paramount to support the wide range of displays web content is consumed on.

Some of the biggest issues facing SVG today is support within IE9-11, both desktop and mobile. IE does not support referencing SVG files externally - so the contents of the file need to be inlined in your HTML document. Also IE fails to scale SVG files appropriately. For these reasons, we will still leverage a JS library to help us manage SVGs across vendors.

_Which library is that, how is it used, how does this work with Modernizr?_

## Video

*   Native Video Player & Considerations
*   Responsive Video Container

Video is still a terribly complex feature to implement successfully accross all the browsing vendors and devices they run on. That's why it's recommended to always use a video hosting service such as YouTube or Vimeo to not only host the video content but to serve within a video player.

But for browsers and devices that support the HTML 5 standard implementation, video can be added to a site with relative ease. _We will explore this more as part of our Video component - this requires not only an HTML implementation, but a JS implementation too._ We should also discuss supported media formats.

Most video today makes use of a 16:9 ratio, and some still use 4:3\. To make a video responsive we can take our knowledge of the video format and adjust the container accordingly. The two utility classes are **ratio-16x9** and **ratio-4x3**.

The child element should be either an iframe, video, or image. It will be positioned absolutely, so if it doesn't share the same aspect ratio, it will appear stretched.

TBD.

<!-- <div class="flex ratios">
<div>
<div class="ratio-16x9 -styleguide">![16:9 Ratio Image](http://placehold.it/640x360/ffffff/cccccc/?text=16:9)</div>
</div>
<div>
<div class="ratio-4x3 -styleguide">![4:3 Ratio Image](http://placehold.it/640x480/ffffff/cccccc/?text=4:3)</div>
</div>
</div> -->

The following example showcases a video from YouTube, inside of an **iframe**.

TBD.

<!--
<div class="flex ratios">
<div>
<div class="ratio-16x9 -styleguide"><iframe width="560" height="315" src="https://www.youtube.com/embed/aHjpOzsQ9YI" frameborder="0" allowfullscreen=""></iframe></div>
</div>
<div>
<div class="ratio-4x3 -styleguide"><iframe width="560" height="315" src="https://www.youtube.com/embed/aHjpOzsQ9YI" frameborder="0" allowfullscreen=""></iframe></div>
</div>
</div>
 -->

This example showcases a **video** element.

TBD.

<!--
<div class="flex ratios">
<div>
<div class="ratio-16x9 -styleguide"><video controls="controls"><source src="/assets/media/Crystallize%20-%20Lindsey%20Stirling%20(Dubstep%20Violin%20Original%20Song).mp4" type="video/mp4"></video> </div>
</div>
<div>
<div class="ratio-4x3 -styleguide"><video controls="controls"><source src="/assets/media/Crystallize%20-%20Lindsey%20Stirling%20(Dubstep%20Violin%20Original%20Song).mp4" type="video/mp4"></video> </div>
</div>
</div>
</div>
-->