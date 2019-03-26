# react-drawable-overlay

> A package for wrapping an element with a drawable canvas.

[![NPM](https://img.shields.io/npm/v/react-drawable-overlay.svg)](https://www.npmjs.com/package/react-drawable-overlay) [![JavaScript Style Guide](https://img.shields.io/badge/code_style-standard-brightgreen.svg)](https://standardjs.com)

## Install

```bash
npm install --save react-drawable-overlay
```

## Usage

```jsx
import React, { Component } from "react"
import DrawableOverlay from "react-drawable-overlay"

class Example extends Component {
  renderDrawableContent = () => (
    <div style={{ height: 500, width: 1000 }}>
      <p>Content that can be drawn on</p>
    </div>
  )

  render() {
    return (
      <DrawableOverlay
        renderDrawableContent={renderDrawableContent}
        defaultBrushColor="#000"
      >
        <p>
          Content that cannot be drawn on but still has access to the
          Context-values
        </p>
        <Toolbar />
      </DrawableOverlay>
    )
  }
}
```

## License

MIT © [jimmyhoglund](https://github.com/jimmyhoglund)
