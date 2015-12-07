## Module Ace.Types

#### `AnchorEvent`

``` purescript
type AnchorEvent = { old :: Position, value :: Position }
```

#### `BackgroundTokenizerEvent`

``` purescript
data BackgroundTokenizerEvent
```

#### `DocumentEventType`

``` purescript
data DocumentEventType
  = Insert
  | Remove
```

##### Instances
``` purescript
instance documentEventTypeIsForeign :: IsForeign DocumentEventType
```

#### `showDocumentEventType`

``` purescript
showDocumentEventType :: DocumentEventType -> String
```

#### `readDocumentEventType`

``` purescript
readDocumentEventType :: String -> F DocumentEventType
```

#### `DocumentEvent`

``` purescript
newtype DocumentEvent
  = DocumentEvent { action :: DocumentEventType, start :: Position, end :: Position, lines :: Array String }
```

##### Instances
``` purescript
instance documentEventIsForeign :: IsForeign DocumentEvent
```

#### `PasteEvent`

``` purescript
data PasteEvent
```

#### `NewlineMode`

``` purescript
data NewlineMode
  = Windows
  | Unix
  | Auto
```

#### `showNewlineMode`

``` purescript
showNewlineMode :: NewlineMode -> String
```

#### `readNewlineMode`

``` purescript
readNewlineMode :: String -> F NewlineMode
```

#### `Rules`

``` purescript
data Rules
```

#### `Annotation`

``` purescript
type Annotation = { row :: Int, column :: Int, text :: String, type :: String }
```

#### `Position`

``` purescript
newtype Position
  = Position { row :: Int, column :: Int }
```

##### Instances
``` purescript
instance positionIsForeign :: IsForeign Position
```

#### `getRow`

``` purescript
getRow :: Position -> Int
```

#### `getColumn`

``` purescript
getColumn :: Position -> Int
```

#### `TokenInfo`

``` purescript
type TokenInfo = { value :: String }
```

#### `SearchOptions`

``` purescript
type SearchOptions = { needle :: String, backwards :: Boolean, wrap :: Boolean, caseSensitive :: Boolean, wholeWord :: Boolean, regExp :: Boolean, skipCurrent :: Boolean }
```

#### `ACE`

``` purescript
data ACE :: !
```

#### `Ace`

``` purescript
data Ace
```

#### `Anchor`

``` purescript
data Anchor
```

#### `BackgroundTokenizer`

``` purescript
data BackgroundTokenizer
```

#### `Document`

``` purescript
data Document
```

#### `Editor`

``` purescript
data Editor
```

#### `EditSession`

``` purescript
data EditSession
```

#### `Range`

``` purescript
data Range
```

#### `RangeList`

``` purescript
data RangeList
```

#### `ScrollBar`

``` purescript
data ScrollBar
```

#### `Search`

``` purescript
data Search
```

#### `Selection`

``` purescript
data Selection
```

#### `TextMode`

``` purescript
newtype TextMode
  = TextMode String
```

#### `TokenIterator`

``` purescript
data TokenIterator
```

#### `Tokenizer`

``` purescript
data Tokenizer
```

#### `UndoManager`

``` purescript
data UndoManager
```

#### `VirtualRenderer`

``` purescript
data VirtualRenderer
```

#### `LanguageTools`

``` purescript
data LanguageTools
```

#### `Completer`

``` purescript
data Completer
```


