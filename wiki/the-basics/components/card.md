---
description: A box with image, link, text, and tags
---

# Card

\
👁 [PREVIEW](https://greenelab.github.io/lab-website-template/testbed#card)​

```liquid
{%
    include card.html
    image="images/space.jpg"
    link="https://nasa.gov/"
    title="A Large Card"
    subtitle="A cool card"
    description="A cool description"
    tooltip="A cool tooltip"
    tags="tag A, tag B, tag C"
    repo="greenelab/lab-website-template"
    style="small"
%}
```



| Parameter     | Description                                                                                                                                                                       |
| ------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `image`       | URL to an image for the card.                                                                                                                                                     |
| `link`        | URL to link to when clicking the image or the title of the card.                                                                                                                  |
| `title`       | Title for the card.                                                                                                                                                               |
| `subtitle`    | Subtitle for the card.                                                                                                                                                            |
| `description` | Text to show under the card name. Can contain Markdown. Accepts [arbitrary content](https://greene-lab.gitbook.io/lab-website-template-docs/basics/components#arbitrary-content). |
| `tooltip`     | Text to show when hovering over the card.                                                                                                                                         |
| `tags`        | ​[Tags](https://greene-lab.gitbook.io/lab-website-template-docs/basics/components/tags) to show at the bottom of the card.                                                        |
| `repo`        | GitHub repository to automatically fetch additional [tags](https://greene-lab.gitbook.io/lab-website-template-docs/basics/components/tags) from.                                  |
| `style`       | Visual style of the card. Set to `small` to make the card a bit smaller.                                                                                                          |
