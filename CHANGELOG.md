# Changelog

This is the MuddyBot project changelog! Also the way I version is confusing so its not your fault its mine.

## [1.1.0] - 2025-06-21

Well version 1.1.0 is here now!

### Changed

- Documentation now updated to version 1.1.0
- We have deprecated commands starting with c! and !.
- Emojis are now removed from log files and replaced with their name.
- Now logging logs in new log file after 00:00 UTC
- Now append log messages to the log file
- Now shows date and time in UTC
- Now it sends the message in the channel the user spoke in not the first channel in the list

### Fixed

- Fixed the system file configuration in docs/service.md

### Removed

- Removed the "-v" command line argument which then removes argparse as a dependency
- Removed c!hello command
- Removed --version option since that was kinda redundant
- Removed unnecessary `if __name__ == "__main__:` since I never used them
- Removed the c!mud_curses command
- Removed the c!send_love command
- Removed the !song command
- Removed the !unlurk command
- Removed the welcome message for users

## [1.1.0-rc1] - 2025-06-20

If no major bugs are found this will become version 1.1.0

### Added

- Added a copyright in the m!help command

### Changed

- Changed c! to m! in the m!help commands

### Removed

- Removed c! and ! commands

## [1.0.5+snapshot25w25e] - 2025-06-18

Commands starting with c! and ! will be deprecated in version 1.1.0

### Fixed

- Fixed the m!find_matches command

## [1.0.4+snapshot25w25d] - 2025-06-17

### Added

- Now removes emojis from chat log file

### Removed

- Removed the !unlurk command
- Removed the welcome message for users

## [1.0.3+snapshot25w25c] - 2025-06-16

### FIXED

- Now logging logs in new log file after 00:00 UTC

## [1.0.2+snapshot25w25b] - 2025-06-15

This is our first official snapshot for week 25!

In retrospect I should have changed the name of last weeks snapshot but the past is in the past.

### Changed

- Now append log messages to the log file
- Now shows date and time in UTC
- Commands now start with m! instead of c!, you can still use the old c! for now though

### Fixed

- Now it sends the message in the channel the user spoke in not the first channel in the list
- Fixed the system file configuration in docs/service.md

### Removed

- Removed the "-v" command line argument which then removes argparse as a dependency

## [1.0.1+snapshot25w25a] - 2025-06-11

We our releasing next weeks snapshot a little earlier because of some concerns [Amie](https://www.twitch.tv/amie_k777) had.

### Changed

- Changed the unlurk message and also allows users to unlurk others
- Now we log the bots chats again
- The bot in most circumstances mentions the user now

### Added

- ~~Now checks if message contains hello or hi and says welcome~~
- Added c!find_matches command

### Removed

- Removed c!hello command
- Removed --version option since that was kinda redundant
- Removed unnecessary `if __name__ == "__main__:` since I never used them
- Removed the c!mud_curses command
- Removed the c!send_love command
- Removed the !song command

## [1.0.0] - 2025-06-09

Forgot to put stuff here before I committed. LOL. No change from [1.0.0-rc1](#100-rc1---2025-06-09)

## [1.0.0-rc1] - 2025-06-09

If no major bugs are found in this update it will become version 1.0.0.

### Changed

- The config file is now once again called config.toml
- Changed the logging message format

## [1.0.0+pre2] - 2025-06-09

This is the second prerelease of version [1.0.0](#100---2025-06-09)!

### Changed

- Changed my email in pyproject.toml it was the wrong email LOL.

### Added

- Added a script `muddybot-key` to generate an encryption key.
- Added documentation

## [1.0.0+pre1] - 2025-06-08

This is our first prerelease of version [1.0.0](#100---2025-06-09). Also because of the way we committed code last time [0.1.3](#013snapshot25w24a---2025-06-08)'s code was a little corrupt.

### Changed

- Changed the name of the project to muddybot

### Added

- Added some error handling for when users don't send arguments with commands that require arguments

### Removed

- Removed !wordleonwheels command
- Removed unused except `KeyboardInterrupt:` code block
- Some unused classifiers in pyproject.toml

## [0.1.3+snapshot25w24a] - 2025-06-08

### Changed

- Changed wordsOnStream to wordleonwheels
- Moved Config file stuff to files.py
- Moved time code to make it more accurate
- Now using "%" formatting in logging functions: [logging-fstring-interpolation / W1203](https://pylint.readthedocs.io/en/latest/user_guide/messages/warning/logging-fstring-interpolation.html)
- Put the bot's code in twitch_bot.py
- Changed c!online to c!status
- Moved logging functionality to logger.py
- Automatically stops searching for word when a user correctly guess the word.

### Added

- Added c!mud_curses command
- Added more comments and docstrings
- Added a way to get word into the program :)

### Removed

- Removed 'word' field in config.toml

## [0.1.2+snapshot25w23b] - 2025-06-07

### Added

- Added classifiers in pyproject.toml
- Added channel field to config file
- Added chat message logging

### Changed

- Changed some values in pyproject.toml
- Changed some formatting in CHANGELOG.md
- Deletes log file on startup
- Changed config file from config.json to config.toml
- Changed log file from log.txt to twbot.log

### Fixed

- Fixed some fields in pyproject.toml

## [0.1.1+snapshot25w23a] - 2025-06-06

### Added

- Added command line argument parsing
- Added a response to the boop command

### Changed

- Changed what is logged
- Now correctly is spelled the right way in \_\_main\_\_.py:64

### Fixed

- Fixed logging to console

## [0.1.0] - 2025-06-06

_Initial release_

[0.1.0]: https://github.com/TheCrunching/MuddyBot/releases/tag/v0.1.0
[0.1.1+snapshot25w23a]: https://github.com/TheCrunching/MuddyBot/releases/tag/v0.1.1+snapshot25w23a
[0.1.2+snapshot25w23b]: https://github.com/TheCrunching/MuddyBot/releases/tag/v0.1.2+snapshot25w23b
[0.1.3+snapshot25w24a]: https://github.com/TheCrunching/MuddyBot/releases/tag/v0.1.3+snapshot25w24a
[1.0.0+pre1]: https://github.com/TheCrunching/MuddyBot/releases/tag/v1.0.0+pre1
[1.0.0+pre2]: https://github.com/TheCrunching/MuddyBot/releases/tag/v1.0.0+pre2
[1.0.0-rc1]: https://github.com/TheCrunching/MuddyBot/releases/tag/v1.0.0-rc1
[1.0.0]: https://github.com/TheCrunching/MuddyBot/releases/tag/v1.0.0
[1.0.1+snapshot25w25a]: https://github.com/TheCrunching/MuddyBot/releases/tag/v1.0.1+snapshot25w25a
[1.0.2+snapshot25w25b]: https://github.com/TheCrunching/MuddyBot/releases/tag/v1.0.2+snapshot25w25b
[1.0.3+snapshot25w25c]: https://github.com/TheCrunching/MuddyBot/releases/tag/v1.0.3+snapshot25w25c
[1.0.4+snapshot25w25d]: https://github.com/TheCrunching/MuddyBot/releases/tag/v1.0.4+snapshot25w25d
[1.0.5+snapshot25w25e]: https://github.com/TheCrunching/MuddyBot/releases/tag/v1.0.5+snapshot25w25e
[1.1.0-rc1]: https://github.com/TheCrunching/MuddyBot/releases/tag/v1.1.0-rc1
[1.1.0]: https://github.com/TheCrunching/MuddyBot/releases/tag/v1.1.0
