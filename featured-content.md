---
sidebar_position: 3
---

# Featured Content

## Description

The Featured Content compeonts add real power to your platform page creation. These widgets let you display courses, microlearning, and products in neat blocks. Configure them to show static content or set them up to dynamically exhibit content based on search queries or tags.

✨🎨 [View Component in Storybook](https://thoughtindustries.github.io/helium/?path=/story/packages-featured-content-base--tile-standard-layout) 🎨✨

## Props

### Props for Featured Content

| Name               | Required | Type              | Description               |
| ------------------ | -------- | -----------       | ------------------------- |
| sidebar            | No       | `ReactNode`       | An optional sidebar for the content    |
| sidebarPosition    | No       | `SidebarPosition` | The position of the sidebar, either Left or Right     |
| children           | No       | `ReactNode`       | The actual content tiles    |

### Props for Content Tiles

| Name                | Required | Type              | Description               |
| ------------------  | -------- | -----------       | ------------------------- |
| headerOptions       | No       | `HeaderOptions`   | Various information such as the title of the header     |
| onAddedToQueue      | No       | `Function`        | Function that handles when the "Add to Queue" button is clicked     |
| onClick             | No       | `Function`        | Function that handles click events    |
| desktopColumnCount  | No       | `Number`          | The number of columns in the featured content list     |
| children            | No       | `ReactNode`       | For the individual content tiles    |


## Standard Layout Example
```
import { FeaturedContent, ContentTileStandardLayout, FeaturedContentContentItem } from '@thoughtindustries/featured-content';

const headerOptions = {
    title: 'Feature Content Header'
}

<FeaturedContent>
    <ContentTileStandardLayout 
        headerOptions={headerOptions}
        onAddedToQueue={(item) => Promise.resolve()}
        desktopColumnCount={2}>
        <ContentTileStandardLayout.Item {...itemOne} />
        <ContentTileStandardLayout.Item {...itemTwo} />
        <ContentTileStandardLayout.Item {...itemThree} />
    </ContentTileStandardLayout>
</FeaturedContent>

```

## Descriptive Layout Example
```
import { FeaturedContent,  
    FeaturedContentContentItem, 
    ContentTileDescriptiveLayout } from '@thoughtindustries/featured-content';

<FeaturedContent>
    <ContentTileDescriptiveLayout 
        headerOptions={...headerOptions} 
        desktopColumnCount={3} 
        onAddedToQueue={(item) => Promise.resolve()}>
    <ContentTileDescriptiveLayout.Item {...itemOne} />
    <ContentTileDescriptiveLayout.Item {...itemTwo} />
    <ContentTileDescriptiveLayout.Item {...itemThree} />
  </ContentTileDescriptiveLayout>
</FeaturedContent>
```

## Image Overlay Example
```
import { FeaturedContent, 
    ContentTileImageOverlay,
    FeaturedContentContentItem } from '@thoughtindustries/featured-content';

<FeaturedContent>
  <ContentTileImageOverlay headerOptions={...headerOptions} desktopColumnCount={3} onAddedToQueue={(item) => Promise.resolve()}>
    <ContentTileImageOverlay.Item {...itemOne} />
    <ContentTileImageOverlay.Item {...itemTwo} />
    <ContentTileImageOverlay.Item {...itemThree} />
  </ContentTileImageOverlay>
</FeaturedContent>
```

## Carousel Example
```
import { FeaturedContent,  
    FeaturedContentContentItem, 
    ContentCarousel } from '@thoughtindustries/featured-content';

<FeaturedContent>
  <ContentCarousel headerOptions={...headerOptions}>
    <ContentCarousel.Item {...itemOne} />
    <ContentCarousel.Item {...itemTwo} />
    <ContentCarousel.Item {...itemThree} />
  </ContentCarousel>
</FeaturedContent>
```

## Multi Carousel
```
import { FeaturedContent,  
    FeaturedContentContentItem, 
    ContentMultiCarousel } from '@thoughtindustries/featured-content';

<FeaturedContent>
  <ContentMultiCarousel headerOptions={...headerOptions} desktopColumnCount={3} onAddedToQueue={(item) => Promise.resolve()}>
    <ContentMultiCarousel.Item {...itemOne} />
    <ContentMultiCarousel.Item {...itemTwo} />
    <ContentMultiCarousel.Item {...itemThree} />
  </ContentMultiCarousel>
</FeaturedContent>
```
