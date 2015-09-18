## Module Graphics.WebGL.Shader

#### `addShaderToProgram`

``` purescript
addShaderToProgram :: WebGLProgram -> ShaderType -> String -> WebGL Unit
```

#### `compileShadersIntoProgram`

``` purescript
compileShadersIntoProgram :: String -> String -> WebGL WebGLProgram
```

#### `getAttrBindings`

``` purescript
getAttrBindings :: forall bindings. WebGLProgram -> WebGL {  | bindings }
```

#### `getUniformBindings`

``` purescript
getUniformBindings :: forall bindings. WebGLProgram -> WebGL {  | bindings }
```


