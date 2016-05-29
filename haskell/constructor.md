## tuple
alias a complex double tuple type
```haskell
type ShopItem = (String, Int)
```
## list
alias a complex list type
```haskell
type ShopList = [ShopItem]
```
## enum
```haskell
data Type = Type1 | Type2 | Type3 ...
            deriving (Show , Eq , ...)
```
>the second line declare which classes the Type belong to

## data & type

### difference
**type** means alias a Type which exsisted</br>
**data** means def a new Type which not exsisted
### single constructor
```haskell
data ShopItem = ShopItem String Int
  deriving (Eq, Show)

type ShopItem =(String, Int)
  deriving (Eq, Show)
```
in fact , the Type of ShopItem is:
```haskell
ShopItem :: String -> Int -> ShopItem
```

### multi constructors
example:
```haskell
data Shap = Circle Float |
            Rectangle Float Float
            deriving (Eq, Ord, Show)
```
generic multi algebra Type
```haskell
data Typename
  = Con1 t --- t |
    Con2 t --- t |
           ---
    Conn t --- t
```

### the strongth of data (constructor)
- each member of Type own itself's label
- must be created by constructor **ShopItem**
- Type name will appear in the error info but not Type alias

### the strongth of type (tuple)
- defination is more compact
- can inherit the behaviors of tuple
