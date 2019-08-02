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

# Specification

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
**Example:**
```js
@defun SafeStr say_hi(SafeStr name)
    return SafeStr("Hi there, #{&name}")
@end
```

#### Variable definition
```js
<type> &variable_name
```
**Example:**
```js
SafeInt &age = 29
```





Single direction inheritance
Immutable inheritance
functional oop
progressive