overview
========

>Haskell function is the mapping of input & output

>Haskell function is the combination of functions and expressions

>Haskell funtion has no status

>Definite input means definite output

>Haskell function is first-letter-low-case



The module of Haskell program are the connection of functions , and function is connection of functions or expressions,so at all the Haskell program is expressions flow</br>

the Haskell program are the functions unfold as exprssions</br>

```haskell

input -> func1 -> ...-> funcn -> ouput

```


the generic function def:</br>
======================

```haskell

func :: Type_input_0 ->...Type_input_n -> Type_output

func input_match1 (= output_expression1)
  | bool_exp1    = output_expression2
  | bool_exp2    = output_expression3
  | otherwise    = output_expression4

```

- the last of the Type declaration is the output Type , others are input Type</br>

- left of **=** is the input match,right of **=** is the output expression</br>
- the guard is match one by one , which guard is matched which expression is the output

function connect
=============

```haskell

func :: Type -> Type

func = func1 . func2

```

means：</br>

>input -> func1 -> func2 -> output

>*connect the functions*

function resolve
================

- unfold the function as expression and caculus the whole expession</br>

- variable just the input or output of function , so it is constant</br>

functon reload
==============
- def multi functions(operators) by one name to meet different Type

- means a function(operator) own different behaviors when acting to different Type

function prove
===============
- prove properties of function
- properties is proved by test or prove

function & operator
====================
- operator prefix mode : (opt)
- function midfix mode : 'func'

operators customize
====================
optional symbols:
> ! # $ % & * + . / < = > ? \ ^ | : - ~ </br>
> can't begain with :

```haskell
(&&&) :: Integer -> Integer -> Integer
x &&& y
  | x > y       = y
  | otherwise   = x
```

### generic function
#### ploymorphism
```haskell
lenghth :: [a] -> Int
```
means a generic function meet any list input and Int output
```haskell
fst :: (a,b) -> a
```
means a generic funtion meet double tuple composed by diff Type iuput and first Type of tuple is the output Type
#### reload
