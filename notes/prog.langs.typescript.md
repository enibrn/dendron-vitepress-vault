---
id: ndojo0tfwunn262fl8y5upu
title: TypeScript
desc: Understanding the Fundamentals of TypeScript
updated: 1728246934755
created: 1691236229372
tags:
  - microsoft
  - oop
  - js
vp:
  ogdate: '2022-03-04'
---
TypeScript has emerged as a popular choice among developers, especially in the world of web development. With its strong typing and object-oriented features, TypeScript brings additional safety and maintainability to JavaScript codebases. In this blog post, we'll explore the fundamentals of TypeScript and why it's worth considering for your next project.

## What is TypeScript?

TypeScript is a superset of JavaScript, which means any valid JavaScript code is also valid TypeScript code. It introduces static typing to JavaScript, allowing developers to specify data types for variables, function parameters, and return values. This helps catch errors early during development and makes code more predictable and self-documenting.

## Installing TypeScript

To get started with TypeScript, you'll need to install it globally using Node Package Manager (NPM). Open your terminal or command prompt and run the following command:

```sh
npm install -g typescript
```

## Basic Syntax

TypeScript provides a familiar syntax to JavaScript developers. Here are some basic examples of TypeScript syntax:

### Variable declaration with type annotation

```typescript
let name: string = "John";
let age: number = 30;
let isStudent: boolean = true;
```

### Function with type annotations for parameters and return value

```typescript
function addNumbers(a: number, b: number): number {
  return a + b;
}
```

### Arrays with type annotations

```typescript
let fruits: string[] = ["apple", "banana", "orange"];
```

### Objects with type annotations

```typescript
interface Person {
  name: string;
  age: number;
}

let person: Person = {
  name: "Alice",
  age: 25,
};
```

## Type Inference

TypeScript is designed to infer types when they are not explicitly provided. For example:

```typescript
let score = 100; // TypeScript infers `score` as a number
let message = "Hello"; // TypeScript infers `message` as a string
```

## Compiling TypeScript

To convert TypeScript code to JavaScript, we need to compile it. Use the following command in the terminal:

```sh
tsc app.ts
```

This will create a new file named app.js containing the compiled JavaScript code.

## Benefits of TypeScript

1. **Type Safety**: TypeScript helps catch errors during development by enforcing strict typing rules, reducing bugs and improving code quality.

2. **Code Maintainability**: Strong typing and object-oriented features make the codebase easier to understand and maintain, especially in larger projects.

3. **Enhanced IDE Support**: IDEs can provide better auto-completion, code navigation, and error checking thanks to TypeScript's type information.

4. **Better Collaboration**: TypeScript's type annotations act as documentation, making it easier for team members to collaborate and understand each other's code.

## Dependency injection

Here’s an example of [[prog.patterns.dependency-injection]] in C#:

```typescript
interface IMyDependency {
  writeMessage(message: string): void;
}

class MyDependency implements IMyDependency {
  writeMessage(message: string): void {
    console.log(`MyDependency.writeMessage Message: ${message}`);
  }
}

class Consumer {
  private myDependency: IMyDependency;

  constructor(myDependency: IMyDependency) {
    this.myDependency = myDependency;
  }

  doSomething(): void {
    this.myDependency.writeMessage("Hello World!");
  }
}
```

In this example, the `Consumer` class depends on an interface called `IMyDependency`. The `MyDependency` class implements this interface. The `Consumer` class takes an instance of `IMyDependency` in its constructor. This is called constructor injection.

When the `doSomething()` method is called on the `Consumer` class, it calls the `writeMessage()` method on the instance of `IMyDependency`.

## Conclusion

TypeScript brings the power of static typing and object-oriented programming to JavaScript, providing numerous benefits for developers and projects of all sizes. As you explore TypeScript further, you'll discover more advanced features and techniques that can help you build robust and scalable applications.

If you haven't already, give TypeScript a try in your next project, and you'll likely find that its benefits outweigh the initial learning curve. Happy coding with TypeScript!
