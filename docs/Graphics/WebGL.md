## Module Graphics.WebGL

#### `runWebgl`

``` purescript
runWebgl :: forall eff a. WebGL a -> WebGLContext -> Eff (canvas :: Canvas | eff) (Either WebGLError a)
```

#### `runWebglWithShaders`

``` purescript
runWebglWithShaders :: forall eff attrs uniforms a. (WebGLProgram -> {  | attrs } -> {  | uniforms } -> WebGL a) -> WebGLContext -> String -> String -> Eff (canvas :: Canvas | eff) (Either WebGLError a)
```

#### `debug`

``` purescript
debug :: WebGL Unit
```


