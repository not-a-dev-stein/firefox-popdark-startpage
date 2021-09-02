![image](https://user-images.githubusercontent.com/63420929/131918897-06f5daac-b410-43d4-8f18-9505adc49e21.png)

# firefox-popdark-startpage
A startpage made inicially for Firefox users inspired by Pop_OS's Pop Dark theme.

## What it is
This project is basically a fork of [my other startpage (and firefox CSS theme), based on the Nord colorscheme](https://github.com/not-a-dev-stein/min-nord-firefox). All I did was change the logo for the stock Firefox logo from the [Papirus icon theme](https://github.com/PapirusDevelopmentTeam/papirus-icon-theme) and the colorscheme, to match Pop!_OS's Pop-Dark theme, which is the one I use myself on my system.

## What it can do
It's pretty simple, you have:

* A collection of saved links to quickly click and be wherever you need to be;
* A little temperature counter at the top-right (which I simply couldn't properly port from the Nord theme, so it stays the way it is);
* And a search bar if you press SPACE while it is focused.

## How you can use it, edit it, and make it work just the way you want it
### ELI5
You can use it with your browser this way, which is the only one that I know of, but if you know any more ways to make it work, feel free to open an issue and let's discuss it.

* Fork this repo by clicking the "fork" button on the top right of the GitHub page (I swear to god I need to learn git enough to know how to do it in the terminal);
* If it doesn't have one already, create a new branch for it by clicking on "master" on the middle-top left of the screen, and typing 'gh-pages' in the text box. An option to create it will appear. __That's the branch that will create your webpage, and the one you need to edit for the changes to appear.__
* That's pretty much it. Now, to access the site you just created, it's pretty simple. the link for it will be formatted like this:\
`your-github-username.github.io/startpage_alt2/index.html`, with obviously `your-github-username` being replaced by your GitHub username.
* Now that you have access to it, it's time to change your startpage. You need the [New Tab Override extension](https://addons.mozilla.org/pt-BR/firefox/addon/new-tab-override/?utm_source=addons.mozilla.org&utm_medium=referral&utm_content=search) to make it as the default page for when you open a new tab. Easy as that. If there are other ways to do so feel free to open an issue about it and I'll update the README.

#### To edit the logo and the welcome message
Under `<div class="container">` in the index.html file, you'll find two things you can change. The logo and the welcome message:

* The logo resides in `<div class="logo"><img src="icons/firefox.svg"/></div>` so all you need to do is add the icon you want to the `icons` folder and add it to the file.
* The welcome message lies right under it, in `<h1 class="hello">Bem-vindo!</h1>`, so all you need to do is change `Bem-vindo!` to whatever message you like.

#### To edit the weather location
As the default, I left it with the data from my home town, so you'll need to change that to where you live, which is pretty simple.

* Looking at the index.html, just change the current link `https://www.bbc.com/weather/0/3461408` for the link from the same website from where you live, just open it, search for your city and change the 7 numbers at the end. Easy peasy.

#### To edit the search engine and the links:

Open the index.html with a text editor and it's pretty easy to find the `Pesquise com DuckDuckGo` (It's in Portuguese but you can easily change it for whatever language you use) in the beginning of the file and `https://duckduckgo.com/?q=` under `// Search on enter key event` by the end of it, and the links to everything under the `div class="category"`. You can edit the links, add more of them to each category, add other categories you want, feel free to tune it to what is perfect for you.

### Why you should do better than me
I have literally zero knowledge on HTML and CSS. I'm pretty upfront about that. It's been almost a year and a half since I first created the firefox-nord repo and just recently I've been actually starting to learn the basics of programming, so all I did with that was tinker about until I found something that worked. Pretty much the same carries to this project.

So, if you find any issues, bugs or anything to help make this startpage better, feel free to fork it, mess with it however you want and make a merge request here. I'm 100% open for help.
