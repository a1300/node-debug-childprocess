<!-- TOC -->

- [Debug `spawn` child process in node.js](#debug-spawn-child-process-in-nodejs)
  - [1 Over Command Line](#1-over-command-line)
    - [1.1 First start the program:](#11-first-start-the-program)
    - [1.2 Then open a new terminal and execute in the same directory:](#12-then-open-a-new-terminal-and-execute-in-the-same-directory)

<!-- /TOC -->


## Debug `spawn` child process in node.js

### 1 Over Command Line

#### 1.1 First start the program:

```bash
node index.js
```

That outputs that the debugger for the `child.js` file is listening on `127.0.0.1:9228`:  

```bash
stderr: Debugger listening on ws://127.0.0.1:9228/ee24da83-fa84-4dab-bc7f-287a47341b1d
For help see https://nodejs.org/en/docs/inspector
```

#### 1.2 Then open a new terminal and execute in the same directory:  

```bash
node inspect 127.0.0.1:9228
```
