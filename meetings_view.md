# <MeetingsView/>

## Description
The `<MeetingsView/>` component displays all the meetings of an ILT or ViLT content type in a list and calender view. This makes it easier for learners to see when meetings take place.

### Example code

```tsx
import { MeetingsView } from '@thoughtindustries/meetings-view';

export function MyComponent() {
  // ...

  return (
    <MeetingsView
        id='adce-de45-5622-dasxs'
        showRating='true'
        showCustomFields='true'
        showSubmitRating='flase'/>
  );
}
```

## Props

| Name               | Required | Type         | Description               |
| ------------------ | -------- | -----------  | ------------------------- |
| id                 | Yes      | `ID`         | The ID of the article     |
| showRating         | Yes      | `Boolean`    | Show or hide the rating of the article      |
| showCustomFields   | Yes      | `Boolean`    | Show or hide the custom fields |
| showSubmitRating   | Yes      | `Boolean`    | Enable or disable learners to submit new ratings     |