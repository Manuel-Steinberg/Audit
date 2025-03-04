# UI & UX:

- [ ] provide the language meta attribute (`lang="de_DE"` and `hreflang`)
- [ ] use CSS cursor property
- [ ] place opposite elements ("Delete" / "Add") far away from each other
- [ ] use space between related buttons/button-groups
- [ ] put related things together
- [ ] do not hide mandatory input fields
- [ ] right click popups safe traveling distance with the mouse
- [ ] avoid reCaptcha
- [ ] popup elements should be ordered by plausability of clicking
- [ ] use microinteractions wisely
- [ ] good CSS doesn´t need _!important_ declaration
- [ ] let user customaize the page in a certain way, e.g. background-color
- [ ] give your development domain a different favicon than production
- [ ] use grid for layout and flexbox for content
- [ ] use progressive JPEG
- [ ] be unique
- [ ] use consistent icon-set
- [ ] add enough space between contrary action buttons, e.g. Cancel/Submit (best opposite side)
- [ ] use occasion-related design, e.g. snow at winter times
- [ ] use _object-fit/object-position_ CSS3 filter
- [ ] use storytelling forms
- [ ] show form tips
- [ ] do not depend on color only
- [ ] do not block zoom
- [ ] rediscover the alt attribute
- [ ] add subtitles and captions to your videos
- [ ] semantics = accessibility
- [ ] use the right mark-up
- [ ] do not split login process
- [ ] use input types!
- [ ] use autofocus wisely, e.g., above the fold only 
- [ ] use `spellcheck="true"` for certain inputs
- [ ] use `search` as input type for search to get the “clear” button
- [ ] use roles when necessary
- [ ] follow web accessibility standards
- [ ] do not use Autoplay
- [ ] use thumb navigation
- [ ] do not put logins in modals
- [ ] create tappable areas for mobile view
- [ ] do not forget _letter-spacing_
- [ ] do not use _:hover_ 
- [ ] provide screen reader meta data (e.g., `aria-current="page"` or `aria-sort="ascending"`)
- [ ] move groups closer to each other, e.g., headlines and content
- [ ] do A/B-Testing
- [ ] use `fieldset`to group controls
- [ ] use labels for every input field
- [ ] reduce number of required fields
- [ ] use neutral color for neutral actions, e.g. Cancel button
- [ ] use tranparency instead of greyout disabled buttons
- [ ] avoid disabled buttons, only show active buttons
- [ ] keep a good contrast always
- [ ] use color-palettes (max. 5)
- [ ] write `alt` text like you are talking to a friend
- [ ] use font-palettes (max. 2)
- [ ] use less _border_
- [ ] Less animations / moving objects
- [ ] use color variants of your product as background
- [ ] provide detailed status of activites
- [ ] remove stock photos (use authentic photos of real people and products)
- [ ] use videos only if it makes a difference
- [ ] use `poster` attribute for videos
- [ ] never autoplay media
- [ ] label icons
- [ ] use icons with selling point character
- [ ] limit external fonts to two
- [ ] get rid of progress bars
- [ ] do not use _pointer-events:none_ for labels within CSS
- [ ] use `<meter>` for quantities
- [ ] use `<mark>` element rather `<span>` for highlighting
- [ ] make links obvious
- [ ] make like-section personal, e.g. famous person bought this as well
- [ ] add key feature to product title, e.g. shorts made with bio-wool
- [ ] add pain point as subtitle, e.g. not noticeable when you wear it
- [ ] use SVG for icons, not icon fonts
- [ ] optimize `@media print` (do not ignore it - people print pages)
- [ ] use `.preventDefault()` for JS event listeners.
- [ ] avoid `target="_blank" in anchors
- [ ] use numeric seperators for large numbers (1_000_000) for readibility
- [ ] interactive elements should disable `user-select` for inner content
- [ ] use `-webkit-font-smoothing: antialiased` and `text-rendering: optimizeLegibility` for fonts
- [ ] do not style browser scrollbar
- [ ] use `text-wrap: balance;` for balanced line-breaks
- [ ] use `title` HTML element to respect the current status of your website
- [ ] use `text-box-trim` for text balancing

## Snippets

```HTML
<form action="#" method="post">
    <fieldset>
      <legend>Register</legend>
      <section>
        <label for="username">Username</label>
        <input id="username" type="text" name="username" placeholder="Username" autocomplete="username" required>
      </section>
      <section>
        <label for="email">Email</label>
        <input id="email" type="email" name="email" placeholder="Email" autocomplete="email" required>
      </section>
      <section>
        <label for="password">Password</label>
        <input id="password" type="password" name="password" placeholder="Password" required>
      </section>
      <section>
        <input type="hidden" name="csrf">
        <button type="submit">Register</button>
      </section>
    </fieldset>
  </form>
```

```CSS
/* Spot layout quirks easily*/

* {
  outline: 1px solid red; 
}
```

```CSS
/* Spot missing alt-attr for images*/

mg[alt=""],
img:not([alt]) {
    outline: 5px dashed red;
}
```


```JS
/* Event Handler != Event Listener */

document.getElementById("myButton").addEventListener("click", function(event){
  event.preventDefault()
});
```


## External Resources:

- [Sign-in form best practices](https://web.dev/sign-in-form-best-practices) ⭐
- [Everything you wanted to know about CTA buttons](https://medium.com/email-industry-news/everything-you-wanted-to-know-about-email-cta-buttons-98807ab98806#.8sf0xg32l)
- [Design Better Forms](https://uxdesign.cc/design-better-forms-96fadca0f49c#.nctmmhrc6)
- [8 simple rules for a robust, scalable CSS architecture](https://github.com/jareware/css-architecture)
- [How to create effective push notifications](https://uxplanet.org/how-to-create-effective-push-notifications-c80f80420453#.t4f6rcyqd)
- [10 guidelines to improve your web accessibility](https://aerolab.co/blog/web-accessibility/)
- [Designing Efficient Web Forms](https://www.smashingmagazine.com/2017/06/designing-efficient-web-forms/)
- [7 Practical Tips for Cheating at Design](https://medium.com/refactoring-ui/7-practical-tips-for-cheating-at-design-40c736799886)
- [Making Future Interfaces: Unusual Shapes](https://youtu.be/eCHt8zsbCT4)
- [How to improve UX of web forms](http://maxsnitser.com/blog/how-to-improve-ux-of-web-forms)
- [A UX Guide For Designing Error Pages](https://blog.prototypr.io/a-ux-guide-for-designing-error-pages-fb9ced1f1c8a)
- [Making the abbr element work for touchscreen, keyboard, and mouse](https://bitsofco.de/making-abbr-work-for-touchscreen-keyboard-mouse/)
- [HTML5 input inputmodes](https://developer.mozilla.org/de/docs/Web/HTML/Element/Input#attr-inputmode)
- [Support tables for HTML5, CSS3, etc](https://caniuse.com/)
- [A collection of the best UX and UI practices.](https://www.checklist.design/)
- [Graphs — a bumpy design ride](https://medium.com/@william.bengtsson/learnings-from-designing-graphs-9033e9034ca0)
- [84 cognitive biases you should exploit to design better products](https://www.mobilespoon.net/2019/04/collection-cognitive-biases-how-to-use.html)
- [Some Imaginary CSS](https://cloudfour.com/thinks/some-imaginary-css/)
- [7 Principles of Icon Design](https://medium.com/@minoraxis/7-principles-of-icon-design-e7187539e4a2)
- [Everything You Ever Wanted to Know About inputmode](https://css-tricks.com/everything-you-ever-wanted-to-know-about-inputmode/)
- [Retargeting im E-Commerce: 5 häufige Fehler und wie du sie vermeidest](https://t3n.de/news/retargeting-e-commerce-5-fehler-1257793/)
- [Die Grundprinzipien von Website-Usability](https://99designs.de/blog/web-digitales-design/website-usability/)
- [100 underline/overlay animations | The ultimate CSS collection](https://dev.to/afif/100-underline-overlay-animation-the-ultimate-css-collection-4p40)
- [12 Conversion-Tipps von Top-Profis](https://t3n.de/news/12-conversion-tipps-top-profis-1377113/)
- [How to build better digital experiences with UX writing principles](https://medium.com/sainsburys-digital-experience/how-to-build-better-digital-experiences-with-ux-writing-principles-3c65fcdbcef8)
- [HTML HELL](https://www.htmhell.dev/tips/the-current-page)
- [Access Guide](https://accessguide.io/)
- [A11y Checklist](https://www.a11yproject.com/checklist)
- [WAVE Web Accessibility Evaluation Tool](https://wave.webaim.org/)
- [Building an adaptive favicon](https://web.dev/building-an-adaptive-favicon)
- [Useful Bookmarklets to Boost Web Development](https://css-tricks.com/web-development-bookmarklets/)
- [How we lost 54k GitHub stars](https://httpie.io/blog/stardust)
- [CSS Almanac :focus-within](https://css-tricks.com/almanac/selectors/f/focus-within/)
- [Specify theme context for images](https://codepen.io/Manuel-Steinberg/pen/mdXMrJX)
- [Obscure CSS: Implicit List-Item Counter](https://kizu.dev/list-item-counter/)
- [Scalable CSS](https://chriscoyier.net/2023/01/17/scalable-css/)
- [Accessibility Overview](https://allforwebforall.com/)
