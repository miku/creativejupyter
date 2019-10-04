---
jupyter:
  jupytext:
    formats: ipynb,md
    text_representation:
      extension: .md
      format_name: markdown
      format_version: '1.1'
      jupytext_version: 1.2.4
  kernelspec:
    display_name: u
    language: python
    name: u
---

# Hello Jupytext

Hello World.

Changes are saved in the markdown file as well.

Images are fine, too.

![](logo.jpg)

```python
import pandas as pd
import matplotlib.pyplot as plt
```

```python
link = "https://en.wikipedia.org/wiki/Belgrade"
tables = pd.read_html(link)
```

```python
data = tables[2]
data = data.set_index('Municipality', drop=True)
```

```python
data["Barajevo":"Zvezdara"].plot(kind='pie', y='Population (2011)', figsize=(14, 10));
plt.grid(zorder=0)
plt.legend(loc='center left', bbox_to_anchor=(1.2, 0.5));
```

```python
data["Barajevo":"Zvezdara"].sort_values(by='Population density (per km2)').plot(
    kind='barh', y='Population density (per km2)', figsize=(12, 8), grid=True);
```

```python

```
