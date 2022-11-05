# Heading

![Version](https://img.shields.io/npm/v/@tiptap/extension-heading.svg?label=version) ![Downloads](https://img.shields.io/npm/dm/@tiptap/extension-heading.svg)

The Heading extension adds support for headings of different levels. Headings are rendered with `<h1>`, `<h2>`, `<h3>`, `<h4>`, `<h5>` or `<h6>` HTML tags. By default all six heading levels (or styles) are enabled, but you can pass an array to only allow a few levels. Check the usage example to see how this is done.

Type `# ` at the beginning of a new line and it will magically transform to a heading, same for `## `, `### `, `#### `, `##### ` and `###### `.

## Installation

```
npm install @tiptap/extension-heading
```## Settings

### HTMLAttributes

Custom HTML attributes that should be added to the rendered HTML tag.

```
Heading.configure({
  HTMLAttributes: {
    class: 'my-custom-class',
  },
})
```### levels

Specifies which heading levels are supported.

Default: `[1, 2, 3, 4, 5, 6]`

```
Heading.configure({
  levels: \[1, 2\],
})
```## Commands

### setHeading()

Creates a heading node with the specified level.

```
editor.commands.setHeading({ level: 1 })
```### toggleHeading()

Toggles a heading node with the specified level.

```
editor.commands.toggleHeading({ level: 1 })
```## Keyboard shortcuts

<table>
  <tr>
    <td>
      <p>Command</p>    </td>
    <td>
      <p>Windows/Linux</p>    </td>
    <td>
      <p>macOS</p>    </td>
  </tr>
  <tr>
    <td>
      <p>toggleHeading({ level: 1 })</p>    </td>
    <td>
      <p><code>Control</code> <code>Alt</code> <code>1</code></p>    </td>
    <td>
      <p><code>Cmd</code> <code>Alt</code> <code>1</code></p>    </td>
  </tr>
  <tr>
    <td>
      <p>toggleHeading({ level: 2 })</p>    </td>
    <td>
      <p><code>Control</code> <code>Alt</code> <code>2</code></p>    </td>
    <td>
      <p><code>Cmd</code> <code>Alt</code> <code>2</code></p>    </td>
  </tr>
  <tr>
    <td>
      <p>toggleHeading({ level: 3 })</p>    </td>
    <td>
      <p><code>Control</code> <code>Alt</code> <code>3</code></p>    </td>
    <td>
      <p><code>Cmd</code> <code>Alt</code> <code>3</code></p>    </td>
  </tr>
  <tr>
    <td>
      <p>toggleHeading({ level: 4 })</p>    </td>
    <td>
      <p><code>Control</code> <code>Alt</code> <code>4</code></p>    </td>
    <td>
      <p><code>Cmd</code> <code>Alt</code> <code>4</code></p>    </td>
  </tr>
  <tr>
    <td>
      <p>toggleHeading({ level: 5 })</p>    </td>
    <td>
      <p><code>Control</code> <code>Alt</code> <code>5</code></p>    </td>
    <td>
      <p><code>Cmd</code> <code>Alt</code> <code>5</code></p>    </td>
  </tr>
  <tr>
    <td>
      <p>toggleHeading({ level: 6 })</p>    </td>
    <td>
      <p><code>Control</code> <code>Alt</code> <code>6</code></p>    </td>
    <td>
      <p><code>Cmd</code> <code>Alt</code> <code>6</code></p>    </td>
  </tr>

</table>
## Source code

[packages/extension-heading/](https://github.com/ueberdosis/tiptap/blob/main/packages/extension-heading/)

## Usage

https://embed.tiptap.dev/preview/Nodes/Heading