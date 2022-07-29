# material-color-utilities-python
Python port of material-color-utilities used for Material You colors

Original source code: https://github.com/material-foundation/material-color-utilities

NOTE: This is an **unofficial** port of material-color-utilities from JavaScript to Python

## Usage examples for Themeing
Theme from color:
```
from utils.theme_utils import *

theme = themeFromSourceColor(argbFromHex('#4285f4'))

print(theme)
```

Color from image:
```
from utils.image_utils import *
from utils.string_utils import *

img = Image.open('path/to/image.png')
argb = sourceColorFromImage(img)

print(hexFromArgb(argb))
```

Theme from image:
```
from utils.theme_utils import *

img = Image.open('path/to/image.png')
theme = themeFromImage(img)

print(theme)
```

