## Main Methods

A Java program without a `main` method cannot be run directly using the java command. However, its methods can still be invoked using the `main` method of another class.

## Class Declaration

成员包括方法与变量

- `static` 关键字声明的是类静态成员，可以被类名调用
- 没有 `static` 关键字声明的是类实例成员，只能被类实例调用

## Constructors

Constructors tell Java what to do when a program tries to create an instance of a class, e.g. what it should do when it executes `Dog d = new Dog()`.

## Array Instantiation

`new` 关键字用于创建数组实例

- `int[] arr = new int[10]`

## Command Line Arguments

 For example if we call our program from the command line like this `java ArgsDemo these are command line arguments`, then the `main` method of `ArgsDemo` will have an array containing the Strings "these", "are", "command", "line", and "arguments".
 