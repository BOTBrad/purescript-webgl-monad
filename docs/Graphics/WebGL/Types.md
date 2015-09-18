## Module Graphics.WebGL.Types

#### `WebGLT`

``` purescript
type WebGLT eff a = ReaderT WebGLContext (ErrorT WebGLError eff) a
```

#### `WebGL`

``` purescript
type WebGL a = forall eff. WebGLT (Eff (canvas :: Canvas | eff)) a
```

#### `WebGLError`

``` purescript
data WebGLError
  = ContextLost
  | ErrorCode ErrorCode
  | NullValue String
  | ShaderError String
```

##### Instances
``` purescript
instance showWebGLError :: Show WebGLError
```

#### `WebGLBuffer`

``` purescript
type WebGLBuffer = WebGLBuffer
```

#### `WebGLContext`

``` purescript
type WebGLContext = WebGLContext
```

#### `WebGLContextAttributes`

``` purescript
type WebGLContextAttributes = WebGLContextAttributes
```

#### `WebGLProgram`

``` purescript
type WebGLProgram = WebGLProgram
```

#### `WebGLShader`

``` purescript
type WebGLShader = WebGLShader
```

#### `WebGLUniformLocation`

``` purescript
type WebGLUniformLocation = WebGLUniformLocation
```

#### `Vec2`

``` purescript
data Vec2
  = Vec2 Number Number
```

#### `Vec3`

``` purescript
data Vec3
  = Vec3 Number Number Number
```

#### `Vec4`

``` purescript
data Vec4
  = Vec4 Number Number Number Number
```

#### `Mat2`

``` purescript
data Mat2
  = Mat2 Number Number Number Number
```

#### `Mat3`

``` purescript
data Mat3
  = Mat3 Number Number Number Number Number Number Number Number Number
```

#### `Mat4`

``` purescript
data Mat4
  = Mat4 Number Number Number Number Number Number Number Number Number Number Number Number Number Number Number Number
```

#### `Attribute`

``` purescript
newtype Attribute a
  = Attribute Int
```

#### `Uniform`

``` purescript
newtype Uniform a
  = Uniform WebGLUniformLocation
```

#### `ToWebGLEnum`

``` purescript
class ToWebGLEnum a where
  toWebglEnum :: a -> Int
```

##### Instances
``` purescript
instance toWebglEnumArrayBufferType :: ToWebGLEnum ArrayBufferType
instance toWebglEnumBufferType :: ToWebGLEnum BufferType
instance toWebglEnumBufferUsage :: ToWebGLEnum BufferUsage
instance toWebglEnumDataType :: ToWebGLEnum DataType
instance toWebglEnumDrawMode :: ToWebGLEnum DrawMode
instance toWebglEnumProgramParam :: ToWebGLEnum ProgramParam
instance toWebglEnumShader :: ToWebGLEnum ShaderType
```

#### `FromWebGLEnum`

``` purescript
class FromWebGLEnum a where
  fromWebglEnum :: Int -> a
```

##### Instances
``` purescript
instance fromWebglEnumErrorCode :: FromWebGLEnum ErrorCode
```

#### `ArrayBufferType`

``` purescript
data ArrayBufferType
  = ArrayBuffer
  | ElementArrayBuffer
```

##### Instances
``` purescript
instance toWebglEnumArrayBufferType :: ToWebGLEnum ArrayBufferType
```

#### `BufferType`

``` purescript
data BufferType
  = DepthBuffer
  | ColorBuffer
  | StencilBuffer
```

##### Instances
``` purescript
instance toWebglEnumBufferType :: ToWebGLEnum BufferType
```

#### `BufferUsage`

``` purescript
data BufferUsage
  = DynamicDraw
  | StaticDraw
  | StreamDraw
```

##### Instances
``` purescript
instance toWebglEnumBufferUsage :: ToWebGLEnum BufferUsage
```

#### `DataType`

``` purescript
data DataType
  = Byte
  | UnsignedByte
  | Short
  | UnsignedShort
  | Int
  | UnsignedInt
  | Float
```

##### Instances
``` purescript
instance toWebglEnumDataType :: ToWebGLEnum DataType
```

#### `DrawMode`

``` purescript
data DrawMode
  = Points
  | Lines
  | LineLoop
  | LineStrip
  | Triangles
  | TriangleStrip
  | TriangleFan
```

##### Instances
``` purescript
instance toWebglEnumDrawMode :: ToWebGLEnum DrawMode
```

#### `ErrorCode`

``` purescript
data ErrorCode
  = NoError
  | InvalidEnum
  | InvalidValue
  | InvalidOperation
  | OutOfMemory
  | UnknownError
```

##### Instances
``` purescript
instance fromWebglEnumErrorCode :: FromWebGLEnum ErrorCode
instance showErrorCode :: Show ErrorCode
```

#### `ProgramParam`

``` purescript
data ProgramParam
  = DeleteStatus
  | LinkStatus
  | ValidateStatus
  | AttachedShaders
  | ActiveAttrs
  | ActiveUniforms
```

##### Instances
``` purescript
instance toWebglEnumProgramParam :: ToWebGLEnum ProgramParam
```

#### `ShaderType`

``` purescript
data ShaderType
  = FragmentShader
  | VertexShader
```

##### Instances
``` purescript
instance toWebglEnumShader :: ToWebGLEnum ShaderType
```

#### `BufferData`

``` purescript
data BufferData
  = DataSize Int
  | DataSource Float32Array
```


