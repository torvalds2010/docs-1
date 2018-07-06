# Usage

This is one of the two relevant git repositories for the documentation. This contains all the product documentation.

## Editing

### Locating file

The file structure is defined in mkdocs.yml. The ordering of the pages is done under "pages:".

### Text

The different text can be found in docs/product/something.md.

### Images

In README.md the syntax to include and image can be found after this: ![ name-of-image ]( link-to-image ) ![ eirik ]( docs/img/Eirik-slow-walk.jpg )

In the product folders it is necessary to put "../img/" instead of "img/".

### Tables

In README.md the syntax to create a table can be found beneath this.

| # | Title 1                             | Title 2              |
| - | :---------------------------------- | :------------------- |
| 1 | Some text here                      |                      |
| 2 | Force line<br> breaks<br> like this | More text here       |

### Links

Link syntax can be found after this in README.md: [waterlinked.com](http://waterlinked.com)

## Deploy changes to server

After the changes have been completed run the command "mkdocs gh-deploy". This updates the gh-pages branch which is the one github pages reads the documentation from.
