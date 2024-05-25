---
color: "#8854d0"
---
# Components 
##### [[Projects/Tesseract/Tesseract|Tesseract]]

![[tesseract-logo.png]]

> [!NOTE]
> Content

### Card
> [!info]- *Documentation*
> **Props**
### Hero
> [!info]- Documentation
> **Version** = 1.0.0
> **Props** = favicon | links | burger | container | sx

**Usage**
```js
import { defineVariadicHero } from "t4-ui"

export function MyHero() {
  return defineHero().value({ preset: "default" })
}

export function App(props) {
  return (
    <MyHero {...props}/>
   )
}
```



### FeaturedGallery
> [!info]- Documentation
> **Props** = [favicon | links | burger | container | sx]




### Image
> [!info]- Documentation
> **Props** = [favicon | links | burger | container | sx]



### DetailSummary
> [!info]- Documentation
> **Props** = [favicon | links | burger | container | sx]


# Metadata
> [!info] Meta
> **Project** = [[Projects/Tesseract/Tesseract|Tesseract]]