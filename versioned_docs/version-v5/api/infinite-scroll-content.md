---
sidebar_label: 'ion-infinite-scroll-content'
---

import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';

import Props from '@ionic-internal/component-api/v5/infinite-scroll-content/props.md';
import Events from '@ionic-internal/component-api/v5/infinite-scroll-content/events.md';
import Methods from '@ionic-internal/component-api/v5/infinite-scroll-content/methods.md';
import Parts from '@ionic-internal/component-api/v5/infinite-scroll-content/parts.md';
import CustomProps from '@ionic-internal/component-api/v5/infinite-scroll-content/custom-props.mdx';
import Slots from '@ionic-internal/component-api/v5/infinite-scroll-content/slots.md';

# ion-infinite-scroll-content

The `ion-infinite-scroll-content` component is the default child used by the `ion-infinite-scroll`. It displays an infinite scroll spinner that looks best based on the platform and changes the look depending on the infinite scroll's state. The default spinner can be changed and text can be added by setting the `loadingSpinner` and `loadingText` properties.

## React

The `ion-infinite-scroll-content` component is not supported in React.

## Usage

<Tabs groupId="framework" defaultValue="angular" values={[{ value: 'angular', label: 'ANGULAR' }, { value: 'javascript', label: 'JAVASCRIPT' }, { value: 'stencil', label: 'STENCIL' }, { value: 'vue', label: 'VUE' }]}>

<TabItem value="angular">

```html
<ion-content>
  <ion-infinite-scroll>
    <ion-infinite-scroll-content loadingSpinner="bubbles" loadingText="Loading more data…">
    </ion-infinite-scroll-content>
  </ion-infinite-scroll>
</ion-content>
```

</TabItem>

<TabItem value="javascript">

```html
<ion-content>
  <ion-infinite-scroll>
    <ion-infinite-scroll-content loading-spinner="bubbles" loading-text="Loading more data…">
    </ion-infinite-scroll-content>
  </ion-infinite-scroll>
</ion-content>
```

</TabItem>

<TabItem value="stencil">

```tsx
import { Component, h } from '@stencil/core';

@Component({
  tag: 'infinite-scroll-content-example',
  styleUrl: 'infinite-scroll-content-example.css',
})
export class InfiniteScrollContentExample {
  render() {
    return [
      <ion-content>
        <ion-infinite-scroll>
          <ion-infinite-scroll-content
            loadingSpinner="bubbles"
            loadingText="Loading more data..."
          ></ion-infinite-scroll-content>
        </ion-infinite-scroll>
      </ion-content>,
    ];
  }
}
```

</TabItem>

<TabItem value="vue">

```html
<template>
  <ion-page>
    <ion-content>
      <ion-infinite-scroll>
        <ion-infinite-scroll-content
          loading-spinner="bubbles"
          loading-text="Loading more data…">
        </ion-infinite-scroll-content>
      </ion-infinite-scroll>
    </ion-content>
  </ion-page>
</template>

<script lang="ts">
import {
  IonContent,
  IonInfiniteScroll,
  IonInfiniteScrollContent,
  IonPage
 } from '@ionic/vue';
import { defineComponent } from 'vue';

export default defineComponent({
  components: {
    IonContent,
    IonInfiniteScroll,
    IonInfiniteScrollContent,
    IonPage
  }
});
```

</TabItem>

</Tabs>

## Properties

<Props />

## Events

<Events />

## Methods

<Methods />

## CSS Shadow Parts

<Parts />

## CSS Custom Properties

<CustomProps />

## Slots

<Slots />
