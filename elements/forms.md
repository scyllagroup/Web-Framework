<div class="breadcrumbs">
[Documentation](/) / Elements / Forms
</div>

# Forms

*   Standard form elements include labels, inputs, checkboxes, radios, textareas, and buttons.
*   Form elements have initial, focus, error, success, and disabled states.
*   Non-standard form elements include switches and sliders.
*   Interactive form elements include file uploads and captchas.
*   Forms have initial, processing, error, and success states.

## Standard Form Elements

These standard form elements all use native browser controls: `label`, `textbox`, `textarea`, `dropdown`, `checkbox`, and `radio`. Form elements have natural occuring states: `focused` or `active`, and `disabled`. But they also have logical states that we manage: `valid`, `invalid`, and `processing`.

The two form styles supported is `block` and `table`.

<div class="flex -pad">
<div>
<form><label><span>Email:</span> <input type="text" placeholder="Your@email.com"> </label> <label> <span>Password:</span> <input type="password" placeholder="Secret"> </label> <label> <span>Dropdown:</span> <select> <option>Please select one</option> <option>Option 1</option> <option>Option 2</option> <option>Option 3</option> </select> </label> <label> <span></span> <input type="checkbox"> Checkbox</label> <label> <span></span> <input type="radio"> Radio</label> <label> <span>Comments:</span> <textarea placeholder="Textarea"></textarea> </label> <button>Submit</button></form>
</div>
<div>
<form class="-table"><label><span>Email:</span> <input type="text" placeholder="Your@email.com"> </label> <label> <span>Password:</span> <input type="password" placeholder="Secret"> </label> <label> <span>Dropdown:</span> <select> <option>Please select one</option> <option>Option 1</option> <option>Option 2</option> <option>Option 3</option> </select> </label> <label> <span></span> <input type="checkbox"> Checkbox</label> <label> <span></span> <input type="radio"> Radio</label> <label><span>Comments:</span> <textarea placeholder="Textarea"></textarea></label>
<div><span></span><button>Submit</button></div>
</form>
</div>
</div>

## Non-standard Form Elements

Non-standard form elements are non-native to the browser but can provide a better user experience if supported. Since they are not native and not standard they only exist as a progressive enhancement to regular form elements. These include `dropdown`, `checkbox`, `radio`, `switch`, and `range`.

<div class="flex -pad">
<div>
<div class="select"><span>Please select one</span>
*   Option 1
*   Option 2
*   Option 3
</div>
<div class="select" data-ismultiple="true"><span>Please select one or more</span>
*   Option 1
*   Option 2
*   Option 3
</div>
</div>
<div>
<div>
<div class="checkbox"><span></span>Checkbox</div>
</div>
</div>
<div>
<div class="blocks">
<div class="radio"><span></span>Radio 1</div>
<div class="radio"><span></span>Radio 2</div>
<div class="radio"><span></span>Radio 3</div>
</div>
</div>
</div>
<div class="flex -pad">
<div>
<div class="switch"><span></span>Switch</div>
</div>
</div>
<div class="flex -pad">
<div>
<div class="slider">
<div class="slide"><span class="line"></span><span class="circle"></span></div>
</div>
</div>
<div style="line-height:66px;margin-left:1rem;">Slider</div>
</div>

## Interactive Form Elements

TBD

## Form States

A form has logical states we need to manage as well: `processing`, and `invalid`.