# Running TypeScript File

---

TypeScript is a powerful superset of JavaScript that adds static types and other useful features to the language. However, Node.js does not understand TypeScript natively, so `.ts` files need to be compiled to JavaScript before they can be run. This document outlines the steps to compile and run TypeScript files in a Node.js environment.

## Prerequisites

- Node.js installed on your system.
- TypeScript and `ts-node` installed globally via npm.

## Steps to Run TypeScript Files

### 1. Install TypeScript and `ts-node`

If not already installed, install TypeScript and `ts-node` globally using npm:

```bash
npm install -g typescript ts-node
```

### 2. Initialize Your TypeScript Project
Navigate to your project directory and initialize a TypeScript project:
```bash
tsc --init
```
This command creates a tsconfig.json file with default TypeScript compiler options.

### 3. Write Your TypeScript Code
Create a .ts file in your project, for example index.ts, and write your TypeScript code in this file.

### 4. Compile TypeScript to JavaScript (Optional)
You can manually compile your TypeScript files to JavaScript using the TypeScript compiler:
```bash
tsc [filename]
```
This step is optional if you're using ts-node, as it compiles TypeScript on-the-fly.

### 5. Run Your TypeScript File with ts-node
Instead of compiling TypeScript files manually, you can use ts-node to run your .ts files directly. To run your TypeScript file, use the following command:
```bash
npx ts-node [filename]
```
Replace index.ts with the path to your TypeScript file.