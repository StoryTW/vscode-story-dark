# Story Dark Theme

A dark theme for VS Code inspired by the styles of One Monokai and One Dark Pro.

Supports VS Code 1.143 and later. Includes TextMate syntax colors,
a full ANSI terminal palette, and colors for Git, diffs, inline
hints, sticky scroll, chat, agent sessions, notebooks, and testing.

## Install from Marketplace

In VS Code, open Extensions, search for **Story Dark Theme** by **StoryTW**, install it,
and choose **Story Dark Theme** from **Preferences: Color Theme**.

## Install locally

1. Download or build `story-dark-1.0.0.vsix`.
2. In VS Code, run **Extensions: Install from VSIX...** and select the file.
3. Run **Preferences: Color Theme** and select **Story Dark Theme**.

## Preview and develop

Open this folder in VS Code and press **F5** to launch the **Preview Story Dark**
configuration. In the Extension Development Host, select **Story Dark Theme** from the
color theme picker. Changes to the theme JSON are applied live.

The theme lives in `themes/Story-Dark-color-theme.json`. `color.scss` documents
the palette; it is not compiled or loaded by VS Code.

Syntax highlighting is defined by TextMate rules. User settings and language
extensions can override the resulting colors.

## Build

Use Node.js 22 or later:

```sh
npm ci
npm run package
```

The generated VSIX contains the theme, manifest, icon, license, and documentation.
There is no extension runtime or compilation step.

## Publish

The manifest uses the Marketplace publisher ID `StoryTW`. Build the VSIX with
`npm run package`, then upload it through the publisher management page.
See the [official publishing guide](https://code.visualstudio.com/api/working-with-extensions/publishing-extension)
for Marketplace setup and publishing options.

## License

[MIT](LICENSE)
