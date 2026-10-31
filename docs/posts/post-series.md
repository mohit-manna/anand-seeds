---
layout: page
title: Post Series
subtitle: Posts
menubar: docs_menu
show_sidebar: false
toc: true
---

## Series of Posts

You can make a post a part of a series of posts, linking to the other posts in the series, by creating a `series` data file and then setting the series in each of the post's front matter.

The current post in the list is highlighted to help give context of where you are in the series.

## Blog Series Data File

Start by creating a YAML file in the `_data` directory. This site uses `_data/example_blog_series.yml` for its cauliflower cultivation articles. Give the series a title and, optionally, a description.

## Sections

Next add sections. Each section can have a label (optional) and items. Each item is the title of an existing blog post. If the title is not found then the link will be empty.

If you just want one list without labels, then omit the label and just add the items.

```yaml
title: Cauliflower Cultivation Guides
sections:
  - items:
  - title: Practical Tips for Faster Cauliflower Growth
  - title: How to Get the Best Germination from Cauliflower Seeds
```

Here is a full example with multiple sections with labels.

```yaml
title: Cauliflower Cultivation Guides
description: Practical guides to growing cauliflower, from seed to harvest.
sections:
  - label: Crop Establishment
    items:
      - title: Practical Tips for Faster Cauliflower Growth
      - title: How to Get the Best Germination from Cauliflower Seeds
      - title: When to Sow Cauliflower: Choosing the Right Time
  - label: Crop Management
    items:
      - title: Cauliflower Cultivation Profit and Loss: A Simple Farm Budget
      - title: Cauliflower Plant Care from Transplanting to Harvest
```

## Update your posts

Finally, add the series setting to your front matter in each post you want the series to show in.

```yaml
series: example_blog_series
```