# <AudioPlayer/>

## Description
The `<AudioPlayer/>` component plays audio files for users. It allows audio to be played at multiple speeds and for users to fast forward or rewind

### Example code

```tsx
import { AudioPlayer } from '@thoughtindustries/AudioPlayer';

export function MyComponent() {
  // ...

  return (
    <AudioPlayer id='adce-de45-5622-dasxs'/>
  );
}
```

## Props

| Name               | Required | Type         | Description               |
| ------------------ | -------- | -----------  | ------------------------- |
| source             | Yes      | `String`     | The soure of the audio file     |