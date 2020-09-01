# Dimmer (in development)

Dims the text outside of current line, by reducing the opacity of the text.

![Context](images/context.gif)  

> The **original project** was released by **Cody Hoover** at https://github.com/hoovercj/vscode-dimmer. I've used the project for a long time and in 2019 I decided to [make some contributions](https://github.com/hoovercj/vscode-dimmer/pulls/alefragnani), but the project didn't receive any updates after 2016, and my contributions were not merged. So, I decided to evolve this fork.

# Features

## Available commands

 * `Toggle Dimmer` - Toggle dimmer on/off
 * `Dimmer: Increment Context` - Increments the context lines
 * `Dimmer: Decrement Context` - Decrements the context lines
 * `Dimmer: Increment Opacity` - Increments the opacity
 * `Dimmer: Decrement Opacity` - Decrements the opacity

## Available settings

* Enable/Disable the extension (`false` by default)

```json
   `dimmer.enabled`: 
```

* Decides whether the `ToggleDimmer` command will affect the user (global) or workspace (local) settings. (`user` by default)

```json
   `dimmer.toggleDimmerCommandScope`: 
```

* Opacity percentage for the dimmed text (`50` by default)

```json
   `dimmer.opacity`: 
```

* Number of lines before and current line that are not dimmed (`0` by default)

```json
   `dimmer.context`: 
```

* Delay in milliseconds for dimming the non-selected text (`0` by default)

```json
   `dimmer.delay`: 
```

# Changelog

### 3.0.0 (in development)
- Add commands to Increment and Decrement Context
- Add commands to Increment and Decrement Opacity
- New identity
- New features being planned

### 2.0.0 
- Dim on editor change (e.g. ctrl+tab). Thanks @roblourens
- Highlight context (n lines before/after). Thanks @rebornix
- Breaking: `dimmer.dimSelectedLines` has been replaced by `dimmer.context`. 

### 1.0.0

Initial release

# License

[MIT](LICENSE.md) &copy; Alessandro Fragnani
[MIT](LICENSE.md) &copy; Cody Hoover