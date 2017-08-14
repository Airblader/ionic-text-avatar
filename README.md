# ionic-text-avatar

This package provides a word (or letter) avatar which can be used with Ionic's `ion-avatar` instead of an image.

## Installation

```
npm install --save ionic-text-avatar
# or
yarn add ionic-text-avatar
```

## Usage

Make sure you add `IonTextAvatar` to the `declarations` array of your `app.module.ts`:

```
import { IonTextAvatar } from 'ionic-text-avatar';

@NgModule({
  declarations: [
    IonTextAvatar
  ]
})
export class AppModule {}
```

After that, you can use `ion-text-avatar` within any occurence of `ion-avatar`. Please note that the `ion-avatar` _is_ still required.

## Examples

```
<ion-list>
  <ion-item>
    <ion-avatar item-start>
      <ion-text-avatar>F</ion-text-avatar>
    </ion-avatar>
    Hello, World!
  </ion-item>
  <ion-item>
    <ion-avatar item-start>
      <ion-text-avatar color="secondary">A</ion-text-avatar>
    </ion-avatar>
    Hello, World!
  </ion-item>
</ion-list>

<ion-chip>
  <ion-avatar item-start>
    <ion-text-avatar>Ab</ion-text-avatar>
  </ion-avatar>
  <ion-label>Hello, World!</ion-label>
</ion-chip>
```

The above produces the following output. Please note that the exact colors depend on the theme of your application:

![ion-text-avatar](https://raw.githubusercontent.com/Airblader/ionic-text-avatar/master/screenshot.png)

## Options

`ion-text-avatar` does _not_ truncate the content or provide an automatically generated color. However, the `color` attribute is supported much like most of Ionic's built-in components.

# License

MIT
