# LazyDB Darcula Theme

A [LazyDB](https://github.com/yelog/lazydb) theme inspired by the classic **JetBrains IntelliJ IDEA Darcula** color scheme.

The goal is to bring the familiar low-contrast JetBrains dark UI and SQL syntax highlighting to LazyDB while keeping the interface readable in a terminal.

## Preview


<img width="1903" height="1036" alt="image" src="https://github.com/user-attachments/assets/7d8575a9-17ac-444a-9208-d87575fbc5e3" />


<img width="1913" height="1046" alt="image" src="https://github.com/user-attachments/assets/c4c69c3b-3324-44ac-b9e5-1861b60e6fdd" />


## Installation

Clone the repository:

```bash
git clone https://github.com/lleWelll/lazydb-jetBrains-darcula-theme.git ~/.config/lazydb/themes/llwll_darcula
```

Then start LazyDB with the theme:

```bash
lazydb --theme-file ~/.config/lazydb/themes/llwll_darcula/lazydb-darcula.json
```

LazyDB watches the theme file for changes, so edits can be applied without restarting the application.

## SQL Syntax Highlighting

The LazyDB syntax tokens are mapped approximately as follows:

```text
Keyword          → #CC7832
Identifier       → #A9B7C6
Relation         → #A9B7C6
Relation Alias   → #A9B7C6
Column           → #A9B7C6
Function         → #FFC66D
Number           → #6897BB
Parameter        → #9876AA
Type             → #6897BB
String           → #6A8759
Comment          → #808080
Operator         → #A9B7C6
Punctuation      → #A9B7C6
```

Some LazyDB semantic roles do not have exact IntelliJ IDEA equivalents. Colors for elements such as `action`, `row_updated`, `row_inserted`, and `surface_raised` are therefore mapped to the closest Darcula colors rather than copied directly from a corresponding JetBrains token.

The actual theme file contains all semantic tokens required by LazyDB.

See the [LazyDB configuration documentation](https://github.com/yelog/lazydb/blob/main/docs/configuration.md) for details about external themes.

## Customization

Feel free to modify any color in `lazydb-darcula.json`.

For example, to make the selection slightly brighter:

```json
"selection": "#2D6099"
```

LazyDB reloads watched theme files automatically, making it easy to tune colors while the application is running.

## References

The theme is based on the visual language and color palette of JetBrains Darcula.

* [LazyDB](https://github.com/yelog/lazydb)
* [LazyDB configuration](https://github.com/yelog/lazydb/blob/main/docs/configuration.md)


