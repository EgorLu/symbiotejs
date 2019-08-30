## Symbiote.JS
<img src="./documentation/images/logo_transparent.png" width=250>

<span>
    <img src="https://img.shields.io/badge/build-passing-brightgreen">
    <img src="https://img.shields.io/badge/tests-passing-brightgreen">
    <img src="https://img.shields.io/badge/docker%20build-passing-brightgreen">
    <img src="https://img.shields.io/badge/deployment-passing-brightgreen">
    <img src="https://img.shields.io/badge/downloads-4.6k%2Fmonth-blue">
    <img src="https://img.shields.io/badge/minified%20size-6.65%20kB-blue">
    <img src="https://img.shields.io/badge/node-%3E%3D%2010.16.1-blue">
</span>

# One Symbiote to rule them all
Symbiote.JS brings the best parts of web development while **completely solving** all negative issues that persist in other frameworks.
A **modern**, **deceptively simple**, **multi-paradigm** language that transpiles into **lightweight**, **high performance** JavaScript code.
The Symbiote ecosystem provides **simple**, **elegant** and **efficient** solutions to everyday problems while maintaining type and memory **safety**,
**determinism** and **flexibility** with a **tiny** yet **complex** set of **declarative** expressions that provide a **rich** way to
develop **brilliant**, **multiplatform**, **blazing-fast** **responsive UIs**.
Symbiote **enchances** the development process of **web** and **native** apps while bringing the **fun** back to programming.

# Key Features
- Huge community
- Strong, statical typing
- Cybernetically secure
- Modular
- Easy to learn
- Guaranteed backward compatibility
- Custom elements
- Human-readable
- Internationalization and localization
- Configurable syntax
- Compilator customization via mixins, skins and lootboxes

# Specification

#### Compilation
Symbiote.JS uses a very smart compilation system, transpiling into cross-platform code that can be ran in the most modern web browsers
on all popular Operating Systems.
Compiled code runs thrice as faster when compared to interpreted code, and is less error prone, thanks to the the compiler
finding errors in favor of runtime errors.

Additionally, compiling ready-to-run code is OS friendly and allows rapid deployment of the entire code base.


#### Function definition
```js
@define_function <type> function_name(<type> argument, <type> named=argument, <generic_type> args_array[], <generic_type> named_args_hash)
    return value
@end
```
##### Function definition, short version:
```js
@defun
```

#### Variable definition
```js
<type> &variable_name
```

#### Basic I/O (!muttability warning)
```js
@import <Text_IO.muttablePrint, Text_IO.muttableInput from "Text_IO">

<SafeFunctionPointer> &out = Text_IO.muttablePrint
<SafeFunctionPointer> &in = Text_IO.muttableInput

# Output
&out(SafeStr("Output"))

# Input
&in()
# Or save the value into a variable
<UnsafeGenericType> &foo << &in()
```

#### Control structures
```js
@if (SafeBool(True) .and. SafeBool(False) .or. SafeBool(True))
    return SafeInt(0)
@end
```



# Examples

#### Hello World

**Default compiler skin (SafeOOP)**
```js
@defun SafeVoid helloWorld(SafeVoid immutableNull)
    return SafeStr("Hello World!")
@end
%%document << helloWorld()
```

**Functional compiler skin (HK)**
```js
@module Main(SymbioteHK) where @main::IO(main) => putStrLn SafeStr("Hello, World!")
```

**Functional-Declarative compiler skin (JQ)**
```js
@this.getProgram().getWindow().getDocument().getDOM().getShadowDOM().asMuttable().writeIO(SafeStr("Hello, World!"))
```

**Imperative 1980 compiler skin (AD)**
```js
@with SymbioteAD.Text_IO @use SymbioteAD.Text_IO
@procedure::Hello is @begin
      Put_Line(SafeStr("Hello, world!"))
@end::Hello
```

#### Basic I/O

**Default compiler skin (SafeOOP)**
```js
@import <Text_IO.muttablePrint, Text_IO.muttableInput from "Text_IO">

@defun SafeStr sayHi(SafeStr name)
    return SafeStr("Hi there, #{&name}")
@end

<SafeFunctionPointer> &input = Text_IO.muttableInput
<SafeFunctionPointer> &print = Text_IO.muttablePrint

&print(SafeStr("Please enter your name:\n"))
<SafeStr> &name << SafeCast(toString() => &input())
%%document << helloWorld(&name)
```



# Future support / Current discussions:

- Single direction inheritance
- Immutable inheritance
- Progressive-Abstractive Functional oop