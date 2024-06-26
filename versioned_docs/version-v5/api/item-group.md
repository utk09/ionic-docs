---
sidebar_label: 'ion-item-group'
---

import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';

import Props from '@ionic-internal/component-api/v5/item-group/props.md';
import Events from '@ionic-internal/component-api/v5/item-group/events.md';
import Methods from '@ionic-internal/component-api/v5/item-group/methods.md';
import Parts from '@ionic-internal/component-api/v5/item-group/parts.md';
import CustomProps from '@ionic-internal/component-api/v5/item-group/custom-props.mdx';
import Slots from '@ionic-internal/component-api/v5/item-group/slots.md';

# ion-item-group

Item groups are containers that organize similar items together. They can contain item dividers to divide the items into multiple sections. They can also be used to group sliding items.

## Usage

<Tabs groupId="framework" defaultValue="angular" values={[{ value: 'angular', label: 'Angular' }, { value: 'javascript', label: 'Javascript' }, { value: 'react', label: 'React' }, { value: 'stencil', label: 'Stencil' }, { value: 'vue', label: 'Vue' }]}>

<TabItem value="angular">

```html
<ion-item-group>
  <ion-item-divider>
    <ion-label>A</ion-label>
  </ion-item-divider>

  <ion-item>
    <ion-label>Angola</ion-label>
  </ion-item>
  <ion-item>
    <ion-label>Argentina</ion-label>
  </ion-item>
  <ion-item>
    <ion-label>Armenia</ion-label>
  </ion-item>
</ion-item-group>

<ion-item-group>
  <ion-item-divider>
    <ion-label>B</ion-label>
  </ion-item-divider>

  <ion-item>
    <ion-label>Bangladesh</ion-label>
  </ion-item>
  <ion-item>
    <ion-label>Belarus</ion-label>
  </ion-item>
  <ion-item>
    <ion-label>Belgium</ion-label>
  </ion-item>
</ion-item-group>

<!-- They can also be used to group sliding items -->
<ion-item-group>
  <ion-item-divider>
    <ion-label> Fruits </ion-label>
  </ion-item-divider>

  <ion-item-sliding>
    <ion-item>
      <ion-label>
        <h3>Grapes</h3>
      </ion-label>
    </ion-item>
    <ion-item-options>
      <ion-item-option> Favorite </ion-item-option>
    </ion-item-options>
  </ion-item-sliding>

  <ion-item-sliding>
    <ion-item>
      <ion-label>
        <h3>Apples</h3>
      </ion-label>
    </ion-item>
    <ion-item-options>
      <ion-item-option> Favorite </ion-item-option>
    </ion-item-options>
  </ion-item-sliding>
</ion-item-group>

<ion-item-group>
  <ion-item-divider>
    <ion-label> Vegetables </ion-label>
  </ion-item-divider>

  <ion-item-sliding>
    <ion-item>
      <ion-label>
        <h3>Carrots</h3>
      </ion-label>
    </ion-item>
    <ion-item-options>
      <ion-item-option> Favorite </ion-item-option>
    </ion-item-options>
  </ion-item-sliding>

  <ion-item-sliding>
    <ion-item>
      <ion-label>
        <h3>Celery</h3>
      </ion-label>
    </ion-item>
    <ion-item-options>
      <ion-item-option> Favorite </ion-item-option>
    </ion-item-options>
  </ion-item-sliding>
</ion-item-group>
```

</TabItem>

<TabItem value="javascript">

```html
<ion-item-group>
  <ion-item-divider>
    <ion-label>A</ion-label>
  </ion-item-divider>

  <ion-item>
    <ion-label>Angola</ion-label>
  </ion-item>
  <ion-item>
    <ion-label>Argentina</ion-label>
  </ion-item>
  <ion-item>
    <ion-label>Armenia</ion-label>
  </ion-item>
</ion-item-group>

<ion-item-group>
  <ion-item-divider>
    <ion-label>B</ion-label>
  </ion-item-divider>

  <ion-item>
    <ion-label>Bangladesh</ion-label>
  </ion-item>
  <ion-item>
    <ion-label>Belarus</ion-label>
  </ion-item>
  <ion-item>
    <ion-label>Belgium</ion-label>
  </ion-item>
</ion-item-group>

<!-- They can also be used to group sliding items -->
<ion-item-group>
  <ion-item-divider>
    <ion-label> Fruits </ion-label>
  </ion-item-divider>

  <ion-item-sliding>
    <ion-item>
      <ion-label>
        <h3>Grapes</h3>
      </ion-label>
    </ion-item>
    <ion-item-options>
      <ion-item-option> Favorite </ion-item-option>
    </ion-item-options>
  </ion-item-sliding>

  <ion-item-sliding>
    <ion-item>
      <ion-label>
        <h3>Apples</h3>
      </ion-label>
    </ion-item>
    <ion-item-options>
      <ion-item-option> Favorite </ion-item-option>
    </ion-item-options>
  </ion-item-sliding>
</ion-item-group>

<ion-item-group>
  <ion-item-divider>
    <ion-label> Vegetables </ion-label>
  </ion-item-divider>

  <ion-item-sliding>
    <ion-item>
      <ion-label>
        <h3>Carrots</h3>
      </ion-label>
    </ion-item>
    <ion-item-options>
      <ion-item-option> Favorite </ion-item-option>
    </ion-item-options>
  </ion-item-sliding>

  <ion-item-sliding>
    <ion-item>
      <ion-label>
        <h3>Celery</h3>
      </ion-label>
    </ion-item>
    <ion-item-options>
      <ion-item-option> Favorite </ion-item-option>
    </ion-item-options>
  </ion-item-sliding>
</ion-item-group>
```

</TabItem>

<TabItem value="react">

```tsx
import React from 'react';

import {
  IonItemGroup,
  IonItemDivider,
  IonLabel,
  IonItem,
  IonItemSliding,
  IonItemOptions,
  IonItemOption,
} from '@ionic/react';

const Example: React.FC<{}> = () => (
  <>
    <IonItemGroup>
      <IonItemDivider>
        <IonLabel>A</IonLabel>
      </IonItemDivider>

      <IonItem>
        <IonLabel>Angola</IonLabel>
      </IonItem>
      <IonItem>
        <IonLabel>Argentina</IonLabel>
      </IonItem>
      <IonItem>
        <IonLabel>Armenia</IonLabel>
      </IonItem>
    </IonItemGroup>

    <IonItemGroup>
      <IonItemDivider>
        <IonLabel>B</IonLabel>
      </IonItemDivider>

      <IonItem>
        <IonLabel>Bangladesh</IonLabel>
      </IonItem>
      <IonItem>
        <IonLabel>Belarus</IonLabel>
      </IonItem>
      <IonItem>
        <IonLabel>Belgium</IonLabel>
      </IonItem>
    </IonItemGroup>

    {/*-- They can also be used to group sliding items --*/}
    <IonItemGroup>
      <IonItemDivider>
        <IonLabel>Fruits</IonLabel>
      </IonItemDivider>

      <IonItemSliding>
        <IonItem>
          <IonLabel>
            <h3>Grapes</h3>
          </IonLabel>
        </IonItem>
        <IonItemOptions>
          <IonItemOption>Favorite</IonItemOption>
        </IonItemOptions>
      </IonItemSliding>

      <IonItemSliding>
        <IonItem>
          <IonLabel>
            <h3>Apples</h3>
          </IonLabel>
        </IonItem>
        <IonItemOptions>
          <IonItemOption>Favorite</IonItemOption>
        </IonItemOptions>
      </IonItemSliding>
    </IonItemGroup>

    <IonItemGroup>
      <IonItemDivider>
        <IonLabel>Vegetables</IonLabel>
      </IonItemDivider>

      <IonItemSliding>
        <IonItem>
          <IonLabel>
            <h3>Carrots</h3>
          </IonLabel>
        </IonItem>
        <IonItemOptions>
          <IonItemOption>Favorite</IonItemOption>
        </IonItemOptions>
      </IonItemSliding>

      <IonItemSliding>
        <IonItem>
          <IonLabel>
            <h3>Celery</h3>
          </IonLabel>
        </IonItem>
        <IonItemOptions>
          <IonItemOption>Favorite</IonItemOption>
        </IonItemOptions>
      </IonItemSliding>
    </IonItemGroup>
  </>
);

export default Example;
```

</TabItem>

<TabItem value="stencil">

```tsx
import { Component, h } from '@stencil/core';

@Component({
  tag: 'item-group-example',
  styleUrl: 'item-group-example.css'
})
export class ItemGroupExample {
  render() {
    return [
      <ion-item-group>
        <ion-item-divider>
          <ion-label>A</ion-label>
        </ion-item-divider>

        <ion-item>
          <ion-label>Angola</ion-label>
        </ion-item>
        <ion-item>
          <ion-label>Argentina</ion-label>
        </ion-item>
        <ion-item>
          <ion-label>Armenia</ion-label>
        </ion-item>
      </ion-item-group>

      <ion-item-group>
        <ion-item-divider>
          <ion-label>B</ion-label>
        </ion-item-divider>

        <ion-item>
          <ion-label>Bangladesh</ion-label>
        </ion-item>
        <ion-item>
          <ion-label>Belarus</ion-label>
        </ion-item>
        <ion-item>
          <ion-label>Belgium</ion-label>
        </ion-item>
      </ion-item-group>


      // They can also be used to group sliding items
      <ion-item-group>
        <ion-item-divider>
          <ion-label>
            Fruits
          </ion-label>
        </ion-item-divider>

        <ion-item-sliding>
          <ion-item>
            <ion-label>
              <h3>Grapes</h3>
            </ion-label>
          </ion-item>
          <ion-item-options>
            <ion-item-option>
              Favorite
            </ion-item-option>
          </ion-item-options>
        </ion-item-sliding>

        <ion-item-sliding>
          <ion-item>
            <ion-label>
              <h3>Apples</h3>
            </ion-label>
          </ion-item>
          <ion-item-options>
            <ion-item-option>
              Favorite
            </ion-item-option>
          </ion-item-options>
        </ion-item-sliding>
      </ion-item-group>

      <ion-item-group>
        <ion-item-divider>
          <ion-label>
            Vegetables
          </ion-label>
        </ion-item-divider>

        <ion-item-sliding>
          <ion-item>
            <ion-label>
              <h3>Carrots</h3>
            </ion-label>
          </ion-item>
          <ion-item-options>
            <ion-item-option>
              Favorite
            </ion-item-option>
          </ion-item-options>
        </ion-item-sliding>

        <ion-item-sliding>
          <ion-item>
            <ion-label>
              <h3>Celery</h3>
            </ion-label>
          </ion-item>
          <ion-item-options>
            <ion-item-option>
              Favorite
            </ion-item-option>
          </ion-item-options>
        </ion-item-sliding>
      </ion-item-group>
    ];
  }
}
```

</TabItem>

<TabItem value="vue">

```html
<template>
  <ion-item-group>
    <ion-item-divider>
      <ion-label>A</ion-label>
    </ion-item-divider>

    <ion-item>
      <ion-label>Angola</ion-label>
    </ion-item>
    <ion-item>
      <ion-label>Argentina</ion-label>
    </ion-item>
    <ion-item>
      <ion-label>Armenia</ion-label>
    </ion-item>
  </ion-item-group>

  <ion-item-group>
    <ion-item-divider>
      <ion-label>B</ion-label>
    </ion-item-divider>

    <ion-item>
      <ion-label>Bangladesh</ion-label>
    </ion-item>
    <ion-item>
      <ion-label>Belarus</ion-label>
    </ion-item>
    <ion-item>
      <ion-label>Belgium</ion-label>
    </ion-item>
  </ion-item-group>

  <!-- They can also be used to group sliding items -->
  <ion-item-group>
    <ion-item-divider>
      <ion-label> Fruits </ion-label>
    </ion-item-divider>

    <ion-item-sliding>
      <ion-item>
        <ion-label>
          <h3>Grapes</h3>
        </ion-label>
      </ion-item>
      <ion-item-options>
        <ion-item-option> Favorite </ion-item-option>
      </ion-item-options>
    </ion-item-sliding>

    <ion-item-sliding>
      <ion-item>
        <ion-label>
          <h3>Apples</h3>
        </ion-label>
      </ion-item>
      <ion-item-options>
        <ion-item-option> Favorite </ion-item-option>
      </ion-item-options>
    </ion-item-sliding>
  </ion-item-group>

  <ion-item-group>
    <ion-item-divider>
      <ion-label> Vegetables </ion-label>
    </ion-item-divider>

    <ion-item-sliding>
      <ion-item>
        <ion-label>
          <h3>Carrots</h3>
        </ion-label>
      </ion-item>
      <ion-item-options>
        <ion-item-option> Favorite </ion-item-option>
      </ion-item-options>
    </ion-item-sliding>

    <ion-item-sliding>
      <ion-item>
        <ion-label>
          <h3>Celery</h3>
        </ion-label>
      </ion-item>
      <ion-item-options>
        <ion-item-option> Favorite </ion-item-option>
      </ion-item-options>
    </ion-item-sliding>
  </ion-item-group>
</template>
<script>
  import {
    IonItem,
    IonItemDivider,
    IonItemGroup,
    IonItemOption,
    IonItemOptions,
    IonItemSliding,
    IonLabel,
  } from '@ionic/vue';
  import { defineComponent } from 'vue';

  export default defineComponent({
    components: {
      IonItem,
      IonItemDivider,
      IonItemGroup,
      IonItemOption,
      IonItemOptions,
      IonItemSliding,
      IonLabel,
    },
  });
</script>
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
