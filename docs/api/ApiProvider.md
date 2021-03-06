---
id: ApiProvider
title: ApiProvider
sidebar_label: ApiProvider
hide_title: true
---

# `ApiProvider`

Can be used as a `Provider` if you **do not already have a Redux store**.

```ts title="Basic usage - wrap your App with ApiProvider"
import * as React from 'react';
import { ApiProvider } from '@rtk-incubator/rtk-query';

function App() {
  return (
    <ApiProvider api={api}>
      <Pokemon />
    </ApiProvider>
  );
}
```

:::danger
Using this together with an existing redux store will cause them to conflict with each other. If you are already using Redux, please use follow the instructions as shown in the [Getting Started guide](../introduction/getting-started).
:::

### Example

<iframe src="https://codesandbox.io/embed/rtk-query-apiprovider-iyzme?fontsize=12&hidenavigation=1&module=%2Fsrc%2FApp.tsx&theme=dark"
     style={{ width: '100%', height: '800px', border: 0, borderRadius: '4px', overflow: 'hidden' }}
     title="RTK Query ApiProvider"
     allow="geolocation; microphone; camera; midi; vr; accelerometer; gyroscope; payment; ambient-light-sensor; encrypted-media; usb" 
     sandbox="allow-modals allow-forms allow-popups allow-scripts allow-same-origin"
></iframe>
