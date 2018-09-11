# Custom Jabber Emoticons
_Custom emoticons (made by me) for a few of my co-workers to use in Jabber, along with some common memes and gifs we like to use. Please don't use my artwork without my permission!_
## Instructions
- Clone this repository to:
 - `C:\Program Files (x86)\Cisco Systems\Cisco Jabber` (delete your CustomEmoticons folder first)
 - Or wherever you like, but you'll have to copy everything to either `...\Cisco Jabber\Emoticons` or `...\Cisco Jabber\CustomEmoticons` manually each time you pull
- **Update** Either delete or move everything in the `...\Cisco Jabber\Emoticons` folder
- Restart Jabber
- Enjoy!

### Optional steps
I've included a program to sort the xml file so that certain emoticons can show up at the top of the emoticon selection box in Jabber, for easier/faster picking. If you'd like to sort your emoticons, follow these steps:
- Run `OrganizeEmoticons.exe`
 - The program makes a backup of your file each time it's run, so you can revert to the previous version for whatever reason
- According to the prompt, choose which set you want at the top
- Restart Jabber
- Enjoy!

_Note: If you want to keep them organized, you'll probably have to organize after each pull_

## Adding Things
_Feel free to add memes/gifs to the repo. Follow these steps to do so, if you don't know how to already._
### 1. Add the file
Add whatever file you want to the repo, adding a specific prefix to the file name, depending on what it is:
- `meme_` meme
- `gif_` gif
- `[yourname]_` custom emote
### 2. Add an entry in `emoticonDefs.xml`
Add an entry for the newly added item(s) in the `emoticonDefs.xml` file:
```
<emoticon defaultKey="thisisfine;" image="meme_thisisfine.png" text="This Is Fine" order="36">
    <alt>i'mfine;</alt>
</emoticon>
```
- `defaultKey` Whatever character(s) you want to trigger the emote (no spaces)
  - As a personal convention, I often like to use some word or phrase followed by a semicolon, one because it's easy to type and remember as a programmer, and two so it's harder to accidentally send something you don't mean to when typing normally.
- `image` The file name
- `text` The name of the emote (what shows up in Jabber's emoticon picker box when you hover over an emote)
- `order` The order that the emote shows up in Jabber's emoticon picker box
- `<alt></alt>` Contains additional keys besides `defaultKey` you want to trigger the emote; optional, and there can be as many as you want  

_Note: If you run `OrganizeEmoticons.exe` after adding the entry, it doesn't matter where you put it in the file or what `order` you give it, the program will sort it._

## To Do/Issues
- Gifs forced to a specific size and shape (square) after sending
- More memes!
- Make Alex some emotes (?)
