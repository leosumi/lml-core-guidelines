# Principles

## P.1: Readability and writability are paramount

Why are you using a lightweight markup language ?
The answer is most likely: because it is easy to use.
Writing is straightforward.
Also, the text is not cluttered with unnecessary symbols and is very readable.

## P.2: KISS

Keep it simple, stupid.
You should not have to think too much to write in a lightweight markup language.

## P.3: Less is more

There should be a unique way to write in a specific language.
If multiple syntax are allowed to discribe a particular element, there should be a prefered one.

## P.4: Treat your prose as code

A text is structed.
It has distinct elements like headings, paragraphs, or sentences.
The written document should reflect the structure of the text.
This will make the following principles easy to implement:

### P.4.1: Play nice with your text editor

You should be able to use a code editor to write your text.
Also, you should be able to take advantage of all the functionalities of your editor.

### P.4.2: Parsing should be trivial

Appliying scripts to your text should not be a headache.
This will allow text analysis for instance.
It will also make the following principle an easy accomplishment.

### P.4.3: Play nice with external tools

Shell tools like `wc`, `diff`, or `grep` should return meaningful information.
A version control system like `git` should store meaningful information.
