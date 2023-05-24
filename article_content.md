# <ArticleContent/>

## Description
The `<ArticleContent/>` component shows the content of the article

### Example code

```tsx
import { ArticleContent } from '@thoughtindustries/article-content';

export function MyComponent() {
  // ...

  return (
    <ArticleContent
        id='adce-de45-5622-dasxs'
        showResourceOne='true'
        showResourceTwo='true'
        showDownloadAudio='flase'
        showExternalLink='true'/>
  );
}
```

## Props
| Name          | Required | Type         | Description               |
| ------------- | -------- | -----------  | ------------------------- |
| slug          | Yes      | `Slug`       | The slug of the content                  |
| numberOfItems   | Yes      | `Int`     | The number of related pieces of content to show, a number between 1 - 6    |