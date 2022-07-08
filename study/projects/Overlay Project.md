---
aliases: 
tags: 
date created: 2022-05-16T10:17:41-04:00Z
date modified: 2022-05-16T10:17:42-04:00Z
---

# Obsidian Overlay CSS Snippets

(To my knowledge, these aren't published as of 20220506, but I wrote about them, so…)

(Writing 20220708 - this isn't published yet, but if you're interested, feel free to ping me at gkeener -at- staff -dot- wvnet -dot- edu, or v2keener -at- gmail -dot- com, and I'll see what I can do. It comes down to spending maybe 30 minutes to an hour setting things up how I like it and making sure everything is ready to go 'public'. The project is already on Github.)

Last, and because I love customizing the product as I take notes and/or find something visually distracting, I'm including a project I call "Obsidian Overlay", which is a set of SCSS files rendered to `*.css` that is then copied into a given `.obsidian\snippets\` folder to be used as CSS Snippets in Obsidian.

Overlay is powered by PowerShell, but a Bash script could also easily do the same thing. All of the `deploySASSY.ps1` script is powered by the `sass` interpreter, which listens for file changes, and then updates CSS output files for every/any SCSS file that's updated. There are many settings, all of which should be labelled according to what they *should* do. Whether a given Overlay snippet works is a matter of which theme is being used. All of the overlays I use currently apply to the Default Obsidian theme, and can also work with many other themes. Some options will break other themes. If in doubt, disable all Overlay snippets before switching to view Obsidian with a different theme.
