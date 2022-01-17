<br>

`[🔖] the flowing is a draft document; last updated on Monday, 17 January 2022`

<br>

Rasterize common HTML elements and [Lit](https://github.com/lit/lit)'s HTML templates

![GitHub](https://img.shields.io/github/license/MiloTheirself/module-lit-capture?label=License)
![GitHub issues](https://img.shields.io/github/issues/MiloTheirself/module-lit-capture?label=Issues)
![Discord](https://img.shields.io/discord/494388532270465024?label=Discord)

[...]

<br>

<!--## Documentation

Full documentation is available at [applic.dev](https://applic.dev/outline/module-lit-capture).

<br>-->

## Overview

[...]

<br>

## Usage

This module allows you to easily capture the entire browser page, 

```typescript
import * as litCapture from '@milotheirself/module-lit-capture';

litCapture.capture().then((result) => console.log)
```

<br>

a specific element, 

```typescript
import * as litCapture from '@milotheirself/module-lit-capture';

litCapture.capture({ 
  target: globalThis.document.querySelector('my-custom-element')!, 
  option: { 
    capture: { dpr: 1.25,  inset: "2.5rem", color: '#eaeaea' },
    resolve: { dpr: 3 }
  } 
}).then((result) => console.log) 
```

<br>

or dynamic [lit expressions](https://lit.dev/docs/templates/expressions/) with differing parameters.

```typescript
// [...]
```

<!--```typescript
import { html, css, nothing } from 'lit';
import { context } from '@milotheirself/module-html-capture';
import * as litCapture from '@milotheirself/module-lit-capture';

const myAwesomeTemplate = {
  styles: () => css`
    [...]
  `
  render: (option) => html`
    [...]
  `
}

litCapture
  .context({
    target: myAwesomeTemplate, 
    option: { capture: { dpr: 2 } } 
  })
  .capture({
    render: [
       // frame 1
       {
         greeting: ['Hello', 'World'], 
       },

       // frame 2
       {
         greeting: ['And hello', 'GitHub'],
         caption: 'These are HTML-snippets turning into an PNG image format–',
       }
     ]
  })
  .then((result) => console.log)
```-->

<!--### Contributing

Please see [CONTRIBUTING.md]().-->
