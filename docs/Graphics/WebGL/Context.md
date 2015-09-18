## Module Graphics.WebGL.Context

#### `defaultWebglContextAttrs`

``` purescript
defaultWebglContextAttrs :: WebGLContextAttributes
```

#### `getWebglContextWithAttrs`

``` purescript
getWebglContextWithAttrs :: forall eff. CanvasElement -> WebGLContextAttributes -> Eff (canvas :: Canvas | eff) (Maybe WebGLContext)
```

#### `getWebglContext`

``` purescript
getWebglContext :: forall eff. CanvasElement -> Eff (canvas :: Canvas | eff) (Maybe WebGLContext)
```

#### `canvasElement`

``` purescript
canvasElement :: WebGL CanvasElement
```

#### `drawingBufferHeight`

``` purescript
drawingBufferHeight :: WebGL Number
```

#### `drawingBufferWidth`

``` purescript
drawingBufferWidth :: WebGL Number
```


