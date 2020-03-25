# Core Guidelines

## File name

The best file names are shell friendly.
Limit your character set to the latin alphabet, even if you write in a language that uses other letters.
Avoid using space character, use hyphen instead.
CamelCase is another possibility to separate words, but I find it more difficult to read.
Finally, try to reserve capital letters for abbreviations or accronyms.

## Character encoding

Use UTF-8.
This will avoid problems if you share your files.
Check your text editor to know which encoding it use, but UTF-8 should be chosen by default nowadays.

## Character set

Do not use tab.
If you need to tabulate, use spaces instead of a tab character.
You can configure your editor to expand tab to spaces when the tab key is pressed.
This will limit the number of different blank characters.

## Text structure

Most lightweight markup languages use blank lines to separate paragraphs.
They will also treat a single newline character as a space character.
This implies that you can put one sentence per line.
If you put each sentence on its line, you will respect [P.4](principles.md).

Do not hard wrap long lines.
This will insert random newline character into your file.
Most text editor can choose between soft and hard wrapping.
Soft wrapping allow to visually break long lines, without adding newline character.

Do not write unnecesary white characters.
Trim trailing speces before a newline character.
And you can also remove unnecesary blank lines.
This can be accomplished by most text editor.
