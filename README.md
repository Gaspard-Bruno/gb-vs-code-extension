# Gaspard & Bruno VS Code Extension README

<!-- PROJECT LOGO -->
<br />
<p align="center">
  <a href="https://gaspardbruno.com/">
    <img src="https://raw.githubusercontent.com/Gaspard-Bruno/gb-vs-code-extension/main/images/gaspardbruno.jpeg" alt="Logo">
  </a>

  <h3 align="center">Gaspard Bruno Snippets</h3>
</p>

[![MIT License](https://img.shields.io/apm/l/atomic-design-ui)](https://github.com/Gaspard-Bruno/gb-vs-code-extension/blob/main/LICENSE)
[![GitHub last commit](https://img.shields.io/github/last-commit/Gaspard-Bruno/gb-vs-code-extension)](https://github.com/Gaspard-Bruno/gb-vs-code-extension/graphs/commit-activity)

Extension With Snippets for productivity.

## Getting Started

Install Gaspard Bruno Extension

### Requirements

- VS Studio Code 😎

### Install

```sh
install commands
```

### Usage

#### React-Native Component Typescript

```javascript
gbrnc;
```

```javascript
import React from "react";
import { View } from "react-native";
import { useStylesContext } from "hooks/styles";
import usePolyglot from "hooks/polyglot";
import stylesheets from "./styles";
import { StackScreenProps } from "@react-navigation/stack";

type RootStackParamList = {
  ComponentName: undefined,
};
type Props = StackScreenProps<RootStackParamList, "ComponentName">;

const ComponentName = ({ navigation }: Props) => {
  const [styles] = useStylesContext(stylesheets);
  const t = usePolyglot("ComponentName");

  return <View style={styles.container}></View>;
};

export default ComponentName;
```

#### Styles Typescript

```javascript
gbStyle;
```

```javascript
import { MapTypes } from "/utils/typeTools";

const styles = (variables: AllVariablesType) =>
  MapTypes({
    common: {
      container: {
        flex: 1,
        backgroundColor: variables.surface900Color,
      },
      constants: {},
    },
  });

export default styles;
```

## Roadmap

- Add more snippets (React, ruby, Etc.)
- Add Gifs for README
- Add Gifs for README

## Contributing

Pull requests are welcome! Feel free to open issues and submit PRs, we will review them and answer back as fast as possible.

## 🚀 Authors

- [@FelipeGCastro](https://www.github.com/FelipeGCastro)
- [@jpamarohorta](https://www.github.com/jpamarohorta)

---

## Following extension guidelines

Ensure that you've read through the extensions guidelines and follow the best practices for creating your extension.

- [Extension Guidelines](https://code.visualstudio.com/api/references/extension-guidelines)

## Working with Markdown

**Note:** You can author your README using Visual Studio Code. Here are some useful editor keyboard shortcuts:

- Split the editor (`Cmd+\` on macOS or `Ctrl+\` on Windows and Linux)
- Toggle preview (`Shift+CMD+V` on macOS or `Shift+Ctrl+V` on Windows and Linux)
- Press `Ctrl+Space` (Windows, Linux) or `Cmd+Space` (macOS) to see a list of Markdown snippets

### For more information

- [Visual Studio Code's Markdown Support](http://code.visualstudio.com/docs/languages/markdown)
- [Markdown Syntax Reference](https://help.github.com/articles/markdown-basics/)

**Enjoy!**
