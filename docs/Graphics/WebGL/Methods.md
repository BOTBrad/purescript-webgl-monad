## Module Graphics.WebGL.Methods

#### `attachShader`

``` purescript
attachShader :: WebGLProgram -> WebGLShader -> WebGL Unit
```

#### `bindBuffer`

``` purescript
bindBuffer :: ArrayBufferType -> WebGLBuffer -> WebGL Unit
```

#### `bufferData`

``` purescript
bufferData :: ArrayBufferType -> BufferData -> BufferUsage -> WebGL Unit
```

#### `clear`

``` purescript
clear :: BufferType -> WebGL Unit
```

#### `clearColor`

``` purescript
clearColor :: Number -> Number -> Number -> Number -> WebGL Unit
```

#### `compileShader`

``` purescript
compileShader :: WebGLShader -> WebGL Unit
```

#### `createBuffer`

``` purescript
createBuffer :: WebGL WebGLBuffer
```

#### `createProgram`

``` purescript
createProgram :: WebGL WebGLProgram
```

#### `createShader`

``` purescript
createShader :: ShaderType -> WebGL WebGLShader
```

#### `drawArrays`

``` purescript
drawArrays :: DrawMode -> Int -> Int -> WebGL Unit
```

#### `enableVertexAttribArray`

``` purescript
enableVertexAttribArray :: forall a. Attribute a -> WebGL Unit
```

#### `getError`

``` purescript
getError :: WebGL Int
```

#### `getProgramParameter`

``` purescript
getProgramParameter :: forall a. WebGLProgram -> ProgramParam -> WebGL a
```

#### `isContextLost`

``` purescript
isContextLost :: WebGL Boolean
```

#### `linkProgram`

``` purescript
linkProgram :: WebGLProgram -> WebGL Unit
```

#### `shaderSource`

``` purescript
shaderSource :: WebGLShader -> String -> WebGL Unit
```

#### `uniform1f`

``` purescript
uniform1f :: forall u. Uniform u -> Number -> WebGL Unit
```

#### `uniform1fv`

``` purescript
uniform1fv :: forall u. Uniform u -> Float32Array -> WebGL Unit
```

#### `uniform2f`

``` purescript
uniform2f :: forall u. Uniform u -> Number -> Number -> WebGL Unit
```

#### `uniform2fv`

``` purescript
uniform2fv :: forall u. Uniform u -> Float32Array -> WebGL Unit
```

#### `uniform3f`

``` purescript
uniform3f :: forall u. Uniform u -> Number -> Number -> Number -> WebGL Unit
```

#### `uniform3fv`

``` purescript
uniform3fv :: forall u. Uniform u -> Float32Array -> WebGL Unit
```

#### `uniform4f`

``` purescript
uniform4f :: forall u. Uniform u -> Number -> Number -> Number -> Number -> WebGL Unit
```

#### `uniform4fv`

``` purescript
uniform4fv :: forall u. Uniform u -> Float32Array -> WebGL Unit
```

#### `useProgram`

``` purescript
useProgram :: WebGLProgram -> WebGL Unit
```

#### `vertexAttrib1f`

``` purescript
vertexAttrib1f :: forall a. Attribute a -> Number -> WebGL Unit
```

#### `vertexAttrib1fv`

``` purescript
vertexAttrib1fv :: forall a. Attribute a -> Float32Array -> WebGL Unit
```

#### `vertexAttrib2f`

``` purescript
vertexAttrib2f :: forall a. Attribute a -> Number -> Number -> WebGL Unit
```

#### `vertexAttrib2fv`

``` purescript
vertexAttrib2fv :: forall a. Attribute a -> Float32Array -> WebGL Unit
```

#### `vertexAttrib3f`

``` purescript
vertexAttrib3f :: forall a. Attribute a -> Number -> Number -> Number -> WebGL Unit
```

#### `vertexAttrib3fv`

``` purescript
vertexAttrib3fv :: forall a. Attribute a -> Float32Array -> WebGL Unit
```

#### `vertexAttrib4f`

``` purescript
vertexAttrib4f :: forall a. Attribute a -> Number -> Number -> Number -> Number -> WebGL Unit
```

#### `vertexAttrib4fv`

``` purescript
vertexAttrib4fv :: forall a. Attribute a -> Float32Array -> WebGL Unit
```

#### `vertexAttribPointer`

``` purescript
vertexAttribPointer :: forall a. Attribute a -> Int -> DataType -> Boolean -> Int -> Int -> WebGL Unit
```


