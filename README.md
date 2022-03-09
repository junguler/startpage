## how to use
install the [New Tab Override](https://addons.mozilla.org/en-US/firefox/addon/new-tab-override/) extension for firefox, click on it's icon at the top right, in the option section use local file and upload the html file, open a new tab and close everything else, in firefox settings, choose the `home` button at the left section and in the `homepage and new window` area choose `custom page` and click on `use current pages`

## how to show glyphs?
go to the nerd fonts [website](https://www.nerdfonts.com/) and download the [CaskaydiaCove Nerd Font](https://github.com/ryanoasis/nerd-fonts/releases/download/v2.1.0/CascadiaCode.zip) font and install the windows compatible version (even if you are on linux or mac) and restart your browser

if the glyphs are still not showing open the font manager in your os and find the name the font was installed as exactly and write it in the html file in [line 21](https://github.com/junguler/startpage/blob/main/home.html#L21) and upload the html file again in the extension

## how it looks?

https://user-images.githubusercontent.com/59083599/155002545-221b496f-c48d-4efd-b473-aa435981f295.mp4

## customizing for your needs
adding and removing links is easy, just copy paste an existing line and change it's content or just remove any that you don't want, check the nerd fonts [cheat sheet](https://www.nerdfonts.com/cheat-sheet) for other glyphs and copy the hex value to make a new class in the style section for extra glyphs, here is an example:

![](python_nerd.png)

```
.python:before { content: "\e73c"; }
```

now make a new link for the homepage of the python website

```
<a href="https://www.python.org/"> <i class="nf python"></i>&nbsp; Python</a>
```

## tabliss.json
this startpage was inspired by [tabliss](https://github.com/joelshepherd/tabliss) and i wanted to see if i can re-create it from scratch so i figured if you like the layout but don't want to manually change the html file you can use the json file to import the stylings i have in your tabliss page and change the contents more easily, the biggest differences between my page and tabliss is i'm using nerd fonts glyphs but they are using the more flat [lucide icons](https://lucide.dev/) and of course tabliss doesn't give you an option to apply nesting in your links

please make a backup with the export button first before importing this file otherwise your links and other configs will be erased
