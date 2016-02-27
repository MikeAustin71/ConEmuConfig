# Atom Setup For 'Go'
## Extracted from [Todd McLeod Go Language Course](https://www.udemy.com/learn-how-to-code/learn/#/)
### Atom Setup Recommendations by __Jamal Yusuf__

## Setting up Go with Atom Editor

I am unfortunately not in the camp of wanting to pay money for sublime or webStorm. So I went and figured out how to have all the features you'd get in webstorm/sublime with Golang and set up Atom (A opensource and free) text editor. If you follow the steps below you will have a complete IDE environment that will save you a ton of headache later on. I want to also say that this is a very opinionated post, I am giving you what I'd recommend. Packages under "Optional" list are of course optional. But please make sure you install the required ones.


## Step 1 - Install Atom Editor


## Step 2 - Install required GoLang command line tools

Open your terminal and type:

```
go get -u golang.org/x/tools/cmd/...  
```

and then

```
go get -u github.com/golang/lint/golint
```

and then

```
go get -u github.com/nsf/gocode
```


## Step 3 - Install Atom packages/themes:

QUICK WAY

To install everything I've recommended as is, do the following:

Download the contents of this text to a file and name it "packages.txt"

in terminal go to the directory that the packages.txt lives in and then run the following command:

apm install --packages-file packages.txt

This will install all the Atom packaged I recommended, if you want to manually install them they are linked below.


MANUAL LONGER WAY  

Click "File > Settings" or press "Ctrl+comma" or "Command+comma"

Look for "+ Install" menu item, and click.

Install the following packages by searching for them and hitting the blue "install" button.

REQUIRED PACKAGES:

*autocomplete-go - provides auto-complete of functions/variables for Golang
*go-config - gives access to Gotools via api so other plugins work.
*go-get - lets you know if there is a more recent version of the library/package you are using, also lest you run go get
*go-imports - Auto import Go packages via the goimports tool
*go-plus - add 'gocode' 'gofmt' 'goimoprt' 'go vet' 'go build' and 'go test' into atom.

#### Basically you don't even need to know what those do, they're auto run when you save a file and it makes your code cleaner

*Terminal Plus - allows you to launch a mini terminal panel right within atom. Similar to what Todd is doing in webstorm.
*go-rename - gorename integration

*language-docker - docker syntax highlighting

## OPTIONAL BUT RECOMMENDED:
*atom-beautify -makes your html/css/js etc code beautiful via right click context menu.
*atom-bootstrap3 - syntax completion for bootstrap 3
*auto-detect-indentation - detects your indentation style per file and applies it.
*autoclose-html - automatically close html tags
*color-picker - have a color changer for color values in atom. Right click and click change color and select a color similar to how you would in a graphics program.

*emmet-atom - the must have tool for productivity, you write a lot of html/css you need this. Visit page for more info.

*File-type-icons - gives icons based on filetype in folder video and in tabs.

*highlight-line - highlights the current line (Sublime style)

*highlight-selected - highlights all instances of current double clicked highlighted text in the open document (Sublime feature).

*Linter - will let you know when you've made a mistake in html/css/js really useful for catching mistakes before they happen.
*Linter-csslint - syntax error highlighting for css

*linter-htmlhint - syntax error highlighting for html

*Minimap - sublime like source code preview on side
*Minimap-highlight-selected - displays highlights in current document in minmap

*Pigments - really neat, colors the background of colors like if you write #ffffff it will color it white for background color. Makes following colors easier.

*MiniMap Pigments - displays the pigment colors in the minimap
*Rainbow Tabs - colors the tab text a different color depending on what filetype you are using.


Themes:
*Set UI - dark theme for atom easy on your eyes.
*Monokai Slate - syntax highlighting style, really should be default.


Installing all of the above will give you some much needed breathing room when you are working on some more advance topics. Enjoy!
