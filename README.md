# Obsidian AU Vault
This vault is intended as a public Github repo for for content related to the West Virginia State Technology Conference 2022 presentation on "Note-taking in Obsidian"[^1].

"gAUdlf" means:
- 'g' for "Gustavo"
- 'AU' as the elemental symbol for "gold"
- 'dlf' for my last name, "DeLaFuerza", which is Spanish for 'of the force'

## A Golden Vault

This Github repository is intended as a "golden" Obsidian vault. One can use this or the 'template' version of this vault to have some pre-made things I find handy in my primary, private vault for note-taking.

For instance, I've chosen some plugins I find handy to incorporate as submodules. I've also included the `.obsidian` folder, which has the `*.json` files, CSS, and other support files.

## Vim Mode

Vim is my favorite text editor at the command line. This applies to bash and Powershell. For the most part, `vim` is easy for me to use, so I always apply that mode to Obsidian. It shouldn't impact how one uses Obsidian to take notes, but in case the presentation included some unexplained text editing maneuvers&mdash;so to speak, Vim Mode might explain them. Vim Mode for Obsidian is recommended if you are familiar with and like operating with a command-line text editor like `vim` or `vi`.

## Obsidian Overlay CSS Snippets

Last, and because I love customizing the product as I take notes and/or find something visually distracting, I'm including a project I call "Obsidian Overlay", which is a set of SCSS files rendered to `*.css` that is then copied into a given `.obsidian\snippets\` folder to be used as CSS Snippets in Obsidian. 

Overlay is powered by PowerShell, but a Bash script could also easily do the same thing. All of the `deploySASSY.ps1` script is powered by the `sass` interpreter, which listens for file changes, and then updates CSS output files for every/any SCSS file that's updated. There are many settings, all of which should be labelled according to what they *should* do. Whether a given Overlay snippet works is a matter of which theme is being used. All of the overlays I use currently apply to the Default Obsidian theme, and can also work with many other themes. Some options will break other themes. If in doubt, disable all Overlay snippets before switching to view Obsidian with a different theme.

[^1]: "Note-taking in Obsidian" was presented on behalf of West Virginia Network (WVNET), the company that hosted the conference. Gustavo Keener, a Banner DBA for WVNET, is the author of this content.