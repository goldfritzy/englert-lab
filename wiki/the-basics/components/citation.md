---
description: >-
  A citation for a particular source, with regular citation details and extra
  "rich" details
---

# Citation

\
​👁 [PREVIEW](https://greenelab.github.io/lab-website-template/testbed#citation)​

Typically you'd use this with the [list](https://greene-lab.gitbook.io/lab-website-template-docs/basics/components/list) component, which would automatically read from `citations.yaml` and pass this component the appropriate parameters. But you can also use it stand-alone to manually display individual citations:

```liquid
{%
    include citation.html
    lookup="doi:10.1016/j.csbj.2020.05.017"
    style="rich"
%}
```



| Parameter      | Description                                                                                                                                                                                                                             | Default                    |
| -------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------- |
| `lookup`       | Lookup citation details from `citations.yaml` by `id` or `title`.                                                                                                                                                                       | ​                          |
| `style`        | Visual style of citation. Set to `rich` to show image and more [rich details](https://greene-lab.gitbook.io/lab-website-template-docs/basics/citations#rich-details).                                                                   | Plain card with basic info |
| `title` / etc. | The same basic and rich citation parameters outlined in the [citation examples.](https://greene-lab.gitbook.io/lab-website-template-docs/basics/citations#examples) Retrieved from lookup, or passed automatically from list component. | ​                          |

​
