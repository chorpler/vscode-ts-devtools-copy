<p align="center">
  <img width="150px" src="./images/icon-large.png" alt="Strip TS Copy" />
 <h2 align="center">Strip TS DevTools Copy</h2>
 <p align="center">VSCode plugin to strip types from TypeScript code while copying it.</p>
  <p align="center">
    <a href="https://marketplace.visualstudio.com/items?itemName=anuraghazra.strip-ts-copy">
      <img alt="Visual Studio Marketplace Installs" src="https://img.shields.io/visual-studio-marketplace/i/anuraghazra.strip-ts-copy?color=red">
    </a>
    <a href="https://github.com/anuraghazra/vscode-strip-ts-copy/issues">
      <img alt="Issues" src="https://img.shields.io/github/issues/anuraghazra/vscode-strip-ts-copy?color=0088ff" />
    </a>
    <a href="https://github.com/anuraghazra/vscode-strip-ts-copy/pulls">
      <img alt="GitHub pull requests" src="https://img.shields.io/github/issues-pr/anuraghazra/vscode-strip-ts-copy?color=0088ff" />
    </a>
    
  </p>
  <p align="center"><small>Love the project? Consider sponsoring to help it improve!</small></p>
</p>

### The Problem

"An underdiscussed benefit of JS over TS - I'll frequently test individual functions by pasting them into the browser console. There's no faster feedback loop. You can't do that with TS. JSDoc TS means extra keystrokes, but overall the ergonomics are waaaay better" --[Rich Harris](https://twitter.com/Rich_Harris/status/1440639878065111048)

Rich Harris is totally right about the annoyance of working with TypeScript when you want to quickly test something out in the browser console. Sure, you could try it using [ts-node](https://typestrong.org/ts-node/) or a [tslab](https://github.com/yunabe/tslab) Jupyter notebook or something, but that still takes up valuable time. I want to just copy it from VSCode, paste it into Chrome, and try it out!

Oh, and I always want it to automatically run the `join lines` command to copy the code as a single line, to make it easier to scroll back through previous commands in DevTools. Although "easier" is relative, I suppose, once the lines get long enough...

Oh, and I also don't want to create global variables with `const` or `let`, because that means you can't update it without reloading the browser window. So cont or a 

So ... let's try this out.



### The Solution

strip-ts-devtools-copy is a vscode plugin which simply transpiles the selected code and directly puts it inside of your clipboard.

> Inspired by BenLesh: 
> https://twitter.com/BenLesh/status/1441057916413489156

### Usage

1. Install the plugin from [marketplace](https://marketplace.visualstudio.com/items?itemName=anuraghazra.strip-ts-copy)

  
2. Select a piece of code with TS

3. To copy the transpiled code press
  - In Windows <kbd>ctrl+alt+c</kbd>
  - In Mac <kbd>shift+alt+cmd+c</kbd>

### Local development

1. Clone the repo
2. Install deps
3. Open `Run & Debug (Ctrl+Shift+D)` panel in vscode and hit start debugging button

### TODO

- [ ] Write tests
- [ ] Setup release pipeline