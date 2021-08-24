# ani-cli

This is a fork of [pystardust's old-ani-cli](https://github.com/pystardust/ani-cli/tree/old-ani-cli)
with [Dink4n's Fix](https://github.com/Dink4n/ani-cli) and patching for better query

A cli to browse and watch anime.

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

## Dependencies

* grep
* curl
* sed
* mpv
