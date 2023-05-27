# How to make a Wow Addon

We need a specific file structure with the name of the folder being the same as the name of the file

```
World of Warcraft
|   
└─_beta_
	|
	└─Infetface
		|
		└─Addons
			| 
			└─MyAddon
				| MyAddon.toc
				| MyAddon.lua

```

Inside `MyAddon.toc` we need to add some metadata to include things like the creator, title:
- `## Interface: XXXXX` 
	- What version of WoW we're using. 
	- Get it from a script in on-game: `/run print((select(4, GetBuildInfo())));`
- `## Title: MyAddon`: 
	- The title needs to be the same as the folder name.
- `## Notes: Shows a message "Hello World"`: 
	- What the Addon does.
- `## Author: Me`:
	- Name of Author
- `## Version: 0.0.1`
	- Addon version


The `.toc` file must contain another `.lua` file with the same name as well, this is where we have our code.

Learning how to "deep dive" if that makes any sence. 
