# Markdown

File for testing “Markdown” (specifically GitHub-flavored Markdown (GFM), an extension of CommonMark).

## Admonitions

### GitHub special

These should render as special blocks on GitHub.
See [the official GitHub documentation][alerts] or [the original GitHub discussion][16925].

[alerts]: https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#alerts
[16925]: https://github.com/orgs/community/discussions/16925

> [!NOTE]
> 
> Useful information that users should know, even when skimming content.
> 
> (Originally) Highlights information that users should take into account, even when skimming.

> [!TIP]
> 
> Helpful advice for doing things better or more easily.

> [!IMPORTANT]
> 
> Key information users need to know to achieve their goal.
> 
> (Originally) Crucial information necessary for users to succeed.

> [!WARNING]
> 
> Urgent info that needs immediate user attention to avoid problems.
> 
> (Originally) Critical content demanding immediate user attention due to potential risks.

> [!CAUTION]
> 
> Advises about risks or negative outcomes of certain actions.

### Bolded quotes

The “native” markdown way I naturally used.
Note the double line break for separate paragraphs.

> **Note**  
> 
> Highlights information that users should take into account, even when skimming.

> **Important**
> 
> Crucial information necessary for users to succeed.

> **Warning**
> 
> Critical content demanding immediate user attention due to potential risks.

> **Success**
>
> Success

> **Tip**
>
> Tip

> **Error**
>
> Error

Note that GitHub originally rendered the first three (Note, Important, and Warning) the same as its special syntax.
It only applied to those three words though; it did not work for the other three (Success, Tip, Error).

However, GitHub broke (removed) this in the November 2023 update.

> **Update - 14 November 2023**
>
> - Add support for `[!TIP]` and `[!CAUTION]`.
> - ...
> - Prevent alerts from being nested within other elements.
> - The initial syntax using e.g. `**Note**` isn't supported any longer.
>
> -- <https://github.com/orgs/community/discussions/16925>

This means, we are back to choosing GitHub-only “Alert” syntax vs. native markdown vs. other admonition syntax.

Overall, I **do not** recommend using GitHub’s syntax given the lack of rendering support in nested elements and non-standard design.
Instead, use standard markdown unless you (the author) plan to only render on GitHub and plan to stay up-to-date with this feature.

### Emoji

More recently, I experimented with using emoji to represent the desired display.
I experimented with both symbols and colors.
Colors have English/western-centric, whereas symbols _should_ have universal meaning. 

#### Symbols

> **ℹ️ Note**
>
> Note (information)

> **ℹ Note**
>
> Note (information)

> **‼️ Important**
>
> Important

> **‼ Important**
>
> Important

> **⚠️ Warning**
>
> Warning

> **⚠ Warning**
>
> Warning

> **✅ Success**
>
> Success (or tip)

> **✔ Success**
>
> Success (or tip)

> **⭕ Success**
>
> Success (or tip)

> **◯ Success**
>
> Success (or tip)

> **💡 Tip**
>
> Tip

> **❌ Error**
>
> Error

> **🛑 Danger**
>
> Danger (error, stop)

#### Colors and shapes (new)

A new take on colors and shapes.
Matches the terms from Ascii doc.

> **🔷 Note**
>
> A note (info)

> **🟢 Tip**
>
> A tip (success)

> **🟨 Caution**
> 
> A caution

> **🔺 Warning**
> 
> A warning (error)

#### Colors and shapes (old)

For accessibility reasons, I differed shapes for the colors.
The shapes link (somewhat) to the symbols.

- Diamonds: 🔶 🔷
- Triangles: 🔻 🔺
- Circles: _all_
- Squares: _all_
- Octagon: 🛑 (not a pure emoji shape per se)

> **🟢 Success**
>
> Success (or tip)

> **🟦 Note**
> 
> Note (information)

> **🔶 Warning**
>
> Warning

> **🔻 Error**
>
> Error

> **🛑 Error**
>
> Error

Note that AsciiDoc would use "Caution" for the yellow warning and "Warning" for the red error (I think).

### Directives syntax

This uses the [Generic directives/plugins syntax (CommonMark RFC)](https://talk.commonmark.org/t/generic-directives-plugins-syntax/444).

[Docusaurus](https://docusaurus.io/docs/markdown-features/admonitions) uses this format.
The examples below come from the Docusaurus examples.

:::note

Some **content** with _Markdown_ `syntax`. Check [this `api`](#).

:::

:::tip

Some **content** with _Markdown_ `syntax`. Check [this `api`](#).

:::

:::info

Some **content** with _Markdown_ `syntax`. Check [this `api`](#).

:::

:::caution

Some **content** with _Markdown_ `syntax`. Check [this `api`](#).

:::

:::danger

Some **content** with _Markdown_ `syntax`. Check [this `api`](#).

:::

### Material for MKDocs

The following copies the [Material for MKDocs admonitions syntax](https://squidfunk.github.io/mkdocs-material/reference/admonitions/).

:   !!! note

        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et
        euismod nulla. Curabitur feugiat, tortor non consequat finibus, justo
        purus auctor massa, nec semper lorem quam in massa.

:   !!! abstract

        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et
        euismod nulla. Curabitur feugiat, tortor non consequat finibus, justo
        purus auctor massa, nec semper lorem quam in massa.

:   !!! info

        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et
        euismod nulla. Curabitur feugiat, tortor non consequat finibus, justo
        purus auctor massa, nec semper lorem quam in massa.

:   !!! tip

        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et
        euismod nulla. Curabitur feugiat, tortor non consequat finibus, justo
        purus auctor massa, nec semper lorem quam in massa.

:   !!! success

        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et
        euismod nulla. Curabitur feugiat, tortor non consequat finibus, justo
        purus auctor massa, nec semper lorem quam in massa.

:   !!! question

        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et
        euismod nulla. Curabitur feugiat, tortor non consequat finibus, justo
        purus auctor massa, nec semper lorem quam in massa.

:   !!! warning

        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et
        euismod nulla. Curabitur feugiat, tortor non consequat finibus, justo
        purus auctor massa, nec semper lorem quam in massa.

:   !!! failure

        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et
        euismod nulla. Curabitur feugiat, tortor non consequat finibus, justo
        purus auctor massa, nec semper lorem quam in massa.

:   !!! danger

        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et
        euismod nulla. Curabitur feugiat, tortor non consequat finibus, justo
        purus auctor massa, nec semper lorem quam in massa.

:   !!! bug

        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et
        euismod nulla. Curabitur feugiat, tortor non consequat finibus, justo
        purus auctor massa, nec semper lorem quam in massa.

:   !!! example

        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et
        euismod nulla. Curabitur feugiat, tortor non consequat finibus, justo
        purus auctor massa, nec semper lorem quam in massa.

:   !!! quote

        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et
        euismod nulla. Curabitur feugiat, tortor non consequat finibus, justo
        purus auctor massa, nec semper lorem quam in massa.
