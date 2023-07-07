# FOCUS

## What is it?

`Focus` is actually almost an alias of mpg123, quickly configured to play m3u web radios.

## Installation

### 1. Downloading focus

To get 'focus' you can download it via git:

`$ git clone https://github.com/gabrielproencaalves/focus.git`

Or, by a [.zip file](https://github.com/gabrielproencaalves/focus/archive/refs/heads/main.zip). Unzip it after downloading it:

`$ unzip focus-main.zip`

### 2. Configuring focus

After downloading, you can choose a folder to store the extracted m3u files, and then edit the `focus` file as follows:

1. Insert the 'path' of the newly saved m3u files into the 'M3UPATH' variable. For example:

`M3UPATH="insert the path of your .m3u files here"`

*to*

`M3UPATH="$HOME/Music/my-m3u-files"`

2. Change the `focus` file permissions to an executable file:

`$ chmod +x focus`

3. Move/copy the `focus` executable file to a directory included in the system PATH variable, this makes it possible to run it as a normal program:

`# cp focus /usr/local/bin/`

If the previous steps were performed correctly, the focus program is ready to be used!

## Usage

Using the program is very simple, it necessarily receives an argument, the playlist to be played:

`$ focus [PLAYLIST]`

*e.g.*

`$ focus metal`

To see the available playlists, just run the program without arguments, so it will show you the m3u files located in the directory path defined in the M3UPATH variable:

`$ focus`

*returns*

```bash
USAGE: focus [PLAYLIST]

Available playlists:
  list  of  available
playlists...
```

## External resources

You can get more information through the man page of mpg123:

`man 1 mpg123`
