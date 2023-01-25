# Muzak-TS

This is a rewrite in Typescript, hopefully with improvements, of the Muzak Squeezebox Skill.

This is currently work in progress to get the basic build/test/deploy working. After that works will undertaking completing the necessary work.

Since the original Muzak, Amazon has changed how media (music) content is handle and requires a catalog to be created. This looks far more promising and a better approach.

An additional challenge, and the real motivation for this work, is to get the music playing directly out of Alexa.

### Commands

- Start Player
  Starts the named player using the last played song or playlist
- Stop Player
  Stops the named player
- Set Volume
  Sets the volume of the named player to the given level between 0 and 100
- Increase/decrease volume
  Increases or decreases the volume of the named player by 10
- Sync Players
  Syncs the first named player to the second
- Unsync Player
  Unsyncs the named player
- Whats Playing
  Returns information about the current song playing on the named player
- Name My Players
  Return a list of all the player names in your network
- Randomize Player
  Starts the named player using a random song
- Previous Track
  Plays the previous track using the named player
- Next Track
  Plays the next track using the named player
- Help
  List all the commands that can be said

### Interactive Mode

An interactive mode is supported where multiple commands may be issued in one session. The target player is remembered between requests so that it does not have to be specified. e.g.

- "Alexa open squeezebox"
- "select player1"
- "play"
- "set volume to 25"
- "exit"

## Credits

- This skill uses an enhanced version of Piotr Raczynski's squeezenode Node.JS module. It has been modified to support basic HTTP authentication as well as some additional functionality
