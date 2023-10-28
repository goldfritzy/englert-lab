# 🎨 Customise your Theme





Although this website was configured to Dr. Englert's wishes, y'all may wish to change the theme in the future. In the file `_styles/-theme.scss` you'll find a palette of variables that are repeatedly used throughout the template's styling to achieve a consistent look.&#x20;

Try customizing these values to distinguish your site from others built on this template engine:

<table><thead><tr><th width="189">Property</th><th>Description</th></tr></thead><tbody><tr><td><p><code>primary</code></p><p>etc...</p></td><td><p>The "theme" colors for your site. Two variations for each, light mode and dark mode.</p><p></p><p>Primary = links, buttons, etc.<br>Seconary = tags, etc.<br>Background = background color of sections, tooltips, etc.<br>Background alt= same as background, but applied to every other section<br>Light gray = dividers, icons, etc.<br>Gray = secondary text, icons, etc.<br>Overlay = transparent shadow</p></td></tr><tr><td><code>title</code><br>etc...</td><td>Fonts for certain types of text. Recommended: use quoted font name from <a href="https://fonts.google.com/">Google Fonts</a>. Alternative: include a font file in your repo, make a <a href="https://developer.mozilla.org/en-US/docs/Web/CSS/@font-face">font face</a> for it, and name it here.<br><br>Title = logo text<br>Heading = headings, buttons, cards, features, etc.<br>Body = default body text, paragraphs, lists, etc.<br>Code = Code blocks and inline code</td></tr><tr><td><code>spacing</code></td><td>Line spacing in paragraphs of text. 1 = single spaced, 2 = double space, etc.</td></tr><tr><td><code>rounded</code></td><td>Border radius on buttons, cards, etc. 0 = completely square.</td></tr><tr><td><code>shadow</code></td><td><a href="https://developer.mozilla.org/en-US/docs/Web/CSS/box-shadow">Drop shadow</a> around images, cards, etc.</td></tr></tbody></table>

In other files in `_styles`, you'll occasionally see Sass variables at the top that you can customize, like screen width wrapping points, image sizes, and more.

## Picking colours

Picking good colours, especially ones that work well together is surprisingly hard, so don't do it without help! Here are some amazing color palettes I highly recommend:

{% embed url="https://www.coolors.co/palettes" %}

{% embed url="https://www.materialpalette.com/colors" %}

{% embed url="https://www.tailwindcolor.com" %}
