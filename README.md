okay so this is you install this


1. download the files
2. make a new directory called ~/.config/fastfetch/txt
3. put sonnenrad.txt (or any custom ascii art with the filename ending with .txt) in there
4. OPTIONAL: backup your config file (~/.config/fastfetch/config.jsonc)
5. edit ~/.config/fastfetch/config.jsonc and replace

"type": "builtin",

with

"source": "$(find \"${XDG_CONFIG_HOME:-$HOME/.config}/fastfetch/txt/\" -name \"*.txt\" | shuf -n 1)",

6. enjoy your ascii art!!!
