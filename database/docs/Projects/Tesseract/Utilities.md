---
color: "#0fb9b1"
---
# Utilities
##### [[Projects/Tesseract/Tesseract|Tesseract]]
![[tesseract-logo.png]]

> [!info]- Tesseract UI Utilities Module
>  *A [[Projects/Tesseract/Tesseract|Tesseract]] module for defining style class-sets programmatically.*

## Accessibility
> [!info]- *Accessibility module*
> **Purpose** = *A module for accessibility class-set generation.*
> **Version** = [`v3.5.0`]
> **Status** = [#stable]
> **Params** = [ `screenReaders`]
> 
##### Usage
```ts
import { accessibility } from "t4-utils"

export const myAccessibilitySx = accessibility({
  screenReader: {
    preset: "disabled"
  })
export const myAccessibilitySx = accessibility({
  screenReader: {
    preset: "disabled"
  })
export const myAccessibilitySx = accessibility({
  screenReader: {
    preset: "custom",
    sx: {
    className: "none-sr"
    }
  })

export function Component({ children }) {
  return <div className={myAccessibilitySx.value()}>
           {children}
          </div>
}
```

### ScreenReader
> *a module for screen reader class-sets*.

**Usage**
```ts
import { screenReader } from "t4-utils"

export const myScreenReaderSx = screenReader({
  preset: "default",
  sx: {
     sm: "disabled"
    }
 })

export function Component({ children, sx }) {
  return (<div className={myScreenReaderSx.value()}>
           {children}
          </div>
     )
}
```

## Background
> [!info]- *Background Module*
> **Purpose** = *a module for generating background style class-sets.*
> **Version** = [`v1.0.0`]
> 	**Params** = [ `backgroundAttachment`, `backgroundClip`, `backgrundColor`, `backgroundClip`, `backgroundOrigin`, `backgroundPosition`, `backgroundRepeat`, `backgroundSize`, `backgroundImage`, `gradientColorStops`]
> **Status** = [#unstable]
##### Usage
```ts
import { background } from "t4-utils"

export function Component({ children, sx }) {

const myBackgroundSx = background({
  backgroundColor: {
    preset: gray,
    sx: {
       intensity: sx.background.backgroundColor
     }
  },
  backgroundAttachment: {
     preset: "fixed",
     sx: {
        sm: "sticky" 
     }
  }
})
  return (<div className={myBackgroundSx.value()}>
           {children}
          </div>
     )
}

```
### BackgroundAttachment
> *a module for generating background-attachment class-sets.*

##### Usage
```ts
import { backgroundAttachment } from "t4-utils"

const myBackgroundAttachmentSx: string = backgroundAttachment({
 preset: {
 
 }
})
```
### BackgroundClip
> *a module for generating background-cip class-sets.*

#### Usage
```ts
import { backgroundClip } from "t4-utils"


const myBackgroundClipSx = backgroundClip({

})

```
### BackgroundColor
> *a module for generating background-color class-sets*.
##### Usage
```ts
import { backgroundColor } from "t4-utils"

const backgroundColorSx = backgroundColor({
  preset: "green",
})

const MyComponent = ({ children, sx }) => {

  return (
       <div className={backgroundColorSx(sx.mode)}>
       {children}
       </div>)
}
```
### BackogroundOrigin
> *a module for generating background-origin class-sets*
### BackgroundPosition
> *a module for generating flex-basis class-sets for flex-box.*
### BackgroundRepeat
> *a module for generating flex-basis class-sets for flex-box.*
### BackgroundSize
> *a module for generating flex-basis class-sets for flex-box.*
### BackgroundImage
> *a module for generating flex-basis class-sets for flex-box.*
### GradientColorStops
> *a module for generating flex-basis class-sets for flex-box.*

## Borders
> [!info] *Borders module*
> **Purpose**
### BorderRadius
> *a module for generating border-radius class-sets.*

*Usage*
```ts
import { borderRadius } from "t4-utils-ts"
```
### BorderWidth
> *a module for generating border-radius class-sets.*
### BorderColor
> *a module for generating border-radius class-sets.*
### BorderStyle
> *a module for generating border-radius class-sets.*
### DivideWidth
> *a module for generating border-radius class-sets.*
### DivideColor
> *a module for generating flex-basis class-sets for flex-box.*
### DivideStyle
> *a module for generating border-radius class-sets.*
### OutlineWidth
### OutlineColor
> *a module for generating border-radius class-sets.*
### OutlineOffset
> *a module for generating border-radius class-sets.*
### RingWidth
### RingColor
> *a module for generating border-radius class-sets.*
### RingOffsetWidth
> *a module for generating flex-basis class-sets for flex-box.*
### RingOffsetColor
> *a module for generating flex-basis class-sets for flex-box.*

## Transitions
> [!info]- Transitions module
> **Version*
### TransitionProperty
> *a module for generating flex-basis class-sets for flex-box.*
### TransitionDuration
> *a module for generating flex-basis class-sets for flex-box.*
### TransitionTimingFunction
> *a module for generating flex-basis class-sets for flex-box.*
### TransitionDelay
> *a module for generating flex-basis class-sets for flex-box.*
### Animation
> *a module for generating flex-basis class-sets for flex-box.*

## Effects
> [!info] **Effects Module**
> Content
### BoxShadow
> *a module for generating flex-basis class-sets for flex-box.*
### BoxShadowColor
> *a module for generating flex-basis class-sets for flex-box.*
### Opacity
> *a module for generating flex-basis class-sets for flex-box.*
### MixBlendMode
> *a module for generating flex-basis class-sets for flex-box.*
### BackgroundBlendMode
> *a module for generating flex-basis class-sets for flex-box.*


## Flex
> [!info]- *Flex module*
> **Purpose** = *a module for generating flex-box and flex-grid class-sets.*
> **Version** = [`v1.0.0`]
### FlexBasis
> *a module for generating flex-basis class-sets for flex-box.*

*Usage*
```ts
import { flexBasis } from "t4-utils-ts"

export const myFlexBasisSx: string = flexBasis({
     base: ""
})
```
### FlexDirection
### FlexWrap
> *a module for generating flex-basis class-sets for flex-box.*
### Flex
> *a module for generating flex-basis class-sets for flex-box.*
### FlexGrow
> *a module for generating flex-basis class-sets for flex-box.*
### FlexShrink
> *a module for generating flex-basis class-sets for flex-box.*
### Order
> *a module for generating flex-basis class-sets for flex-box.*
### GridTemplateColumns
> *a module for generating flex-basis class-sets for flex-box.*
### GridColumnStartEnd
> *a module for generating flex-basis class-sets for flex-box.*

### GridTemplateRows
> *a module for generating flex-basis class-sets for flex-box.*
### GridRowStartEnd
> *a module for generating flex-basis class-sets for flex-box.*
### GridAutoFlow
> *a module for generating flex-basis class-sets for flex-box.*
### GridAutoRows
> *a module for generating flex-basis class-sets for flex-box.*
### Gap
> *a module for generating border-radius class-sets.*
### JustifyContent
> *a module for generating border-radius class-sets.*
### JustifyItems
### JustifySelf
### AlginContent
### AlignItems
### AlignSelf
### PlaceContent
### PlaceItems
> *a module for generating border-radius class-sets.*
### PlaceSelf
## Filters
> [!info] Filters Module
> **Version** = `v1.0.0`
##### Usage
```ts
import { filters } from "t4-utils"
```
### Blur
> *a module for generating border-radius class-sets.*
### Brightness
> *a module for generating border-radius class-sets.*
### Contrast
> *a module for generating border-radius class-sets.*
### DropShadow
> *a module for generating border-radius class-sets.*
### Grayscale
> *a module for generating border-radius class-sets.*
### HueRotate
> *a module for generating border-radius class-sets.*
### Invert
> *a module for generating border-radius class-sets.*
### Saturate
> *a module for generating border-radius class-sets.*
### Sepia
### BackdropBlur
> *a module for generating border-radius class-sets.*
### BackdropBrightness
> *a module for generating border-radius class-sets.*
### BackdropContrast
### BackdropGrayscale
> *a module for generating border-radius class-sets.*
### BackdropHueRotate
> *a module for generating border-radius class-sets.*
### BackdropInvert
> *a module for generating border-radius class-sets.*
### BackdropOpacity
> *a module for generating border-radius class-sets.*
### BackdropSaturate
> *a module for generating border-radius class-sets.*
### BackdropSepia
> *a module for generating border-radius class-sets.*

## Transform
> [!info]- *Transform module*
> **Version** =  [`1.0.0`]

```js
import { transform } from "t4-utils"

const myTransform = transform({
   scale: {
   preset: 2
   },
   rotate: {
   preset: 180 
   },
   translate: {
    preset: 10
   }
})
```

### Scale
> a module for transform scaling.
### Rotate

### Translate

### Skew

### Transform Origin

## Typography
> [!info]- Typography Module
> **Purpose** =
> **Version**

*Usage*
```ts
import { typography } from "t4-utils-ts"

const mySx: string = typography({
   fontFamily: "",
   
})
```
### FontFamily
>  A control for fontFamily

**Usage**
```ts

import { fontFamily } from "t4-utils-ts"

export const mySx: string = fontFamily("Monospace");
```
### FontSize
> A module for font size 

**Usage**

```ts

import { fontSize } from "t4-utils-ts"

const myFontSizeSx: string = fontSize(3)
```
### FontSmoothing
### FontStyle
### FontWeight
### FontVariantNumeric
### LetterSpacing
### LineClamp
### LineHeight
### ListStyleImage
### ListStylePosition
### ListStyleType
### TextAlign
### TextDecoration
### TextDecorationColor
### TextDecorationStyle
### TextDecorationThickness
### TextUnderlineOffset
### TextTransform
### TextOverflow
### TextIndent
### VerticalAlign
### Whitespace
### WordBreak
### Hyphens
### Content


## Layout
> [!info]- *Layout Module*
> **Purpose**  =
> **Version** = [`v1.0.0`]
> **Params** = `aspectRatio` , `container` , `columns` , `breakAfter` , `breakBefore`
### AspectRatio
> *a module for generating aspect-ratio class-sets*

*Usage*
```ts
import { aspectRatio } from "t4-utils-ts"

export const myAspectRatioSx: string = aspectRatio({
base: 0
})
```
### Container
> *a module for generating container class-sets*

```ts
import { container } from "t4-utils-ts"

export const myContainerSx: string = container({
      base: ""
})
```
### Columns
> *a module for generating columns class-sets.*

*Usage*
```ts
import { columns } from "t4-utils-ts"
```
### BreakAfter
> *a module for generating break-after class-sets.*

```ts
import { breakAfter } from "t4-utils"
```
### BreakBefore
> *a module for generating border-radius class-sets.*
### BreakInside
> *a module for generating border-radius class-sets.*
### BoxDecorationBreak
> *a module for generating border-radius class-sets.*
### BoxSizing
> *a module for generating border-radius class-sets.*
### Display 
> *a module for generating border-radius class-sets.*
### Floats
> *a module for generating border-radius class-sets.*
### Clear
> *a module for generating border-radius class-sets.*
### Isolation
> *a module for generating border-radius class-sets.*
### ObjectFit
> *a module for generating border-radius class-sets.*
### ObjectPosition
> *a module for generating border-radius class-sets.*
### Overflow
> *a module for generating border-radius class-sets.*
### OverscrollBehavior
> *a module for generating border-radius class-sets.*
### Position
> *a module for generating border-radius class-sets.*
#### Top
##### Usage
```ts
import { top } from ""
```
####  Right
##### Usage
```ts
import { top } from ""
```
#### Bottom
##### Usage
```ts
import { top } from ""
```
####  Left
##### Usage
```ts
import { top } from ""
```
### Visibility
> *a module for generating border-radius class-sets.*
### ZIndex
> *a module for generating border-radius class-sets.*

##### Usage
```ts
import { top } from ""
```
### Spacing
>*Purpose** = *a module for generating*
##### Usage
```ts
import { spacing } from "t4-utils"
```
### Padding
> *a module for generating padding class-sets.*

#### Usage
```ts
import { padding } from "t4-utils"

export const myPaddingSx: string = padding({
    base: ""
})
```
### Margin
### SpaceBetween

## Table
> [!info]- *Table module*
> **Purpose** = *a module for generating table class-sets.*
> *Version* = [`v1.0.0`]

**Usage**
```ts
import { table } from "t4-utils"

export const myTablesSx: string = table({
    base: ""
})
```
### BorderCollapse
> *a module for generating border-radius class-sets.*
### BorderSpacing
> *a module for generating border-radius class-sets.*
### TypingLayout
> *a module for generating border-radius class-sets.*
### CaptionSide
> *a module for generating border-radius class-sets.*
> 
## SVG
> [!info]- *Vector Graphics Module*
> **Version** = [`v1.0.0`]
> **Purpose** = []
> **Parameters** = []

**Usage**
```ts
import { svg } from "t4-utils"

const mySVGSx: string = svg({ 
    fill: {},
    stroke: {},
    strokeWidth: {},
})
```
### Fill
> Function to ctronl SVG fill.

**USage**
```ts

import { fill } from "t4-utils-ts"



```
### Stroke
> function tronrol svg stroke
### StrokeWidth
>  fefe 

**Usage**
```ts

import { strokeWidth } from "t4-utils-ts"


export const myStrokeWidthSx: string = strokeWidth(3)
```
## Sizing
> [!info]- *Sizing Module*
>  **Purpose** = *a module for generating sizing class-sets.*
>  **Version** = [`v1.0.0`] 
>  

**Usage**
```ts
import { sizing } from "t4-utils"

export const mySx: string = sizing({ 
     height: {},
     width: {},
     maxHeight,
     maxWidth,
     minHeight,
     minWidth: {}})
```
### Width
> controls eleent widths

**Usage**
```ts
import { width } from "t4-utils"

export const mySx: string = width(5)
```
### Height
> Controls element height. 

**Usage**
```ts

import { height } from "t4-utils-ts"

export const mySx: string = height(3)
```

### MinWidth 
> feff

**Usage**
```ts
import { minWidth } from "t4-utils-ts"



```
### MinHeight
> feffe
### MaxHeight
>  efefef
### MaxWidth
> *a module for generating class-sets *

*Usage*
```ts
import { maxWidth } from "t4-utils-ts"

export const my
```
## Interactivity
> [!info]- *Interactivity module*
> **Purpose** = *a module for generating interactivity class-sets.*
> **Version** = [`v1.0.0`]
> **Status** = [#unstable]

**Usage**
```ts

import { interactivity } from "t4-utils"



```
### AccentColor
>  fef

**Usage**
```ts

import { acces}
```

### Appearance
> *a module for generating border-radius class-sets.*

### Cursor

> *a module for generating border-radius class-sets.*

### Cursor

### CaretColor
> *a module for generating border-radius class-sets.*

### PointerEvents
> *a module for generating border-radius class-sets.*
### Resize
> *a module for generating border-radius class-sets.*
### ScrollBehavior
> *a module for generating border-radius class-sets.*
### ScrollMargin
> *a module for generating border-radius class-sets.*
### ScrollPadding
> *a module for generating border-radius class-sets.*
### ScrollSnapAlign
> *a module for generating border-radius class-sets.*
### ScrollSnapStop
> *a module for generating border-radius class-sets.*
### ScrollSnapType
> *a module for generating border-radius class-sets.*
### TouchAction
> *a module for generating border-radius class-sets.*
### UserSelect
> *a module for generating border-radius class-sets.*
### WillChange
>  a module for generating will-change class-sets. 
#### Usage
```ts
import { willChange } from "t4-utils"

export const myWillChangeSx: string = willChange("");

export function Component({ props, sx }) {
  return (
    <div className={myWillChangeSx, ...sx}>
    </div>
   )
 }
```
## Miscellaneous
> [!info]- *Miscellaneous*
> **Purpose** = *Core module utilities to build stylizers and their parent presets for both parametric & variadic components.*
> **Version** = [`3.0.0`]
> **Date** = 2023-09-17
> **Status** = [#in-progress]

### Utils
```ts
import { defineStylizer, defineStyleSet } from "t4-utils"

export function stylizerA(params) {
 return defineStylizer({
    preset: myPresetsA,
    parameters: params
    })
}

export function stylizerB(params) {
 return defineStylizer({
    preset: myPresetsB,
    parameters: params
    })
}

export function stylizerC(params) {
 return defineStylizer({
    preset: myPresetsC,
    parameters: params
    })
}


export function styleSet(params) {
 return defineStyleSet({
    preset: {...stylizerA,...stylizerB,...stylizerC },
    parameters: params
    })
}

```

### Stylizer
```ts
import { stylizer } from "t4-utils"

const theme = stylizer({
...all presets eficiently loaded
})

```
# Metadata
> [!info]- *Metadata*
> **Project** = [[Projects/Tesseract/Tesseract|Tesseract]]
> **Version** = [`v3.2.0`]
> **NPM Package** = [**🔗Package Link**](https://www.npmjs.com/package/t4-utils)
> **Github** = [**🔗Repository Link**](https://github.com/desirablesolutions/tesseract)
> **Status** = [#in-progress #unstable  ]
> **Purpose** = *The documentation of utility modules for Tesseract UI.*