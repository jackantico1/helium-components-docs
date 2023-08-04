---
sidebar_position: 2
---

# Description

The Catalog allows learners to search and browse for content.

✨🎨 [View Component in Storybook](https://thoughtindustries.github.io/helium/?path=/story/packages-catalog--list) 🎨✨

## Props

### Props for CatalogProvider Component

| Name               | Required | Type                     | Description               |
| ------------------ | -------- | --------------------     | ------------------------- |
| config             | Yes      | `CatalogProviderConfig`  | A config object that controls various aspects of the Catalog     |

### Props for Catalog

| Name               | Required | Type         | Description               |
| ------------------ | -------- | -----------  | ------------------------- |
| onAddedToQueue     | Yes      | `funtion`    | Function that handles when the "Add to Queue" button is clicked      |
| priceFormat        | No       | `function`   | Function that formats how the price is displayed     |

## Examples

### Example with Search Params and Custom Pagination

```
import { Catalog, CatalogProvider } from '@thoughtindustries/catalog';

const config = {
  parsedUrl: {
    pathname: '/catalog',
    searchString: '?query=test'
  }
}

<CatalogProvider config={config}>
  <Catalog
    onAddedToQueue={(item) => Promise.resolve()}
    pagination={({page, pageSize, total, getPageLink}) => <>...</>} />
</CatalogProvider>
```

### Example with a Custom Price Formatter

```
import { Catalog, CatalogProvider } from '@thoughtindustries/catalog';

const config = {
  parsedUrl: {
    pathname: '/catalog',
    searchString: '?query=test'
  }
}

const priceFormat = (priceInCents) => {
  const formatter = new Intl.NumberFormat('en-US', {
      style: 'currency',
      currency: 'USD'
    });
  return formatter.format(priceInCents / 100);
}
<CatalogProvider config={config}>
  <Catalog
    onAddedToQueue={(item) => Promise.resolve()}
    priceFormat={priceFormat} />
</CatalogProvider>
```
