# ani-cli

This is a fork of [pystardust's old-ani-cli](https://github.com/pystardust/ani-cli/tree/old-ani-cli)
with [Dink4n's Fix](https://github.com/Dink4n/ani-cli) and patching for better query

A cli to browse and watch anime with support for different players.

This tool scrapes the site [gogoanime](https://gogoanime.vc).


## Usage

	# watch anime
	ani-cli <query>

	# download anime
	ani-cli -d <query>

	# resume watching anime
	ani-cli -H

Multiple episodes can be viewed/downloaded by giving the episode range like so

	Choose episode [1-13]: 1 6

This would open/download episodes 1 2 3 4 5 6

## Alternative Players
### For VLC
Uncomment the line `#player_fn="vlc"; player_arg="--play-and-exit"` and comment or remove the one just below it.
DISCLAIMER: Some anime don't seem to work with VLC thanks to what I believe is referrer business.

For any other player that accepts terminal input, just modify `player_fn` and `player_arg` and the setsid function to work with Referrers as well.

## Dependencies

* grep
* curl
* sed
* mpv or vlc
* ffmpeg
