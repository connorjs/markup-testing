# Markdown

File for testing “Markdown” (specifically GitHub-flavored Markdown (GFM), an extension of CommonMark).

## Admonitions

### GitHub special

These should render as special blocks on GitHub.
[See the GitHub discussion](https://github.com/orgs/community/discussions/16925#discussioncomment-2827410).

> [!NOTE]  
> Highlights information that users should take into account, even when skimming.

> [!IMPORTANT]  
> Crucial information necessary for users to succeed.

> [!WARNING]  
> Critical content demanding immediate user attention due to potential risks.

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

Note that GitHub renders the above the same as its special syntax.
It only applies to those three words though; it does not work on the following.

> **Success**
>
> Success

> **Tip**
>
> Tip

> **Error**
>
> Error

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

> **❌ Error**
>
> Error

#### Colors and shapes

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
