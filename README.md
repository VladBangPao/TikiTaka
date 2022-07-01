# TikiTaka
## Playing Spanish Football with Files and Data
- Tiki Taka is a Spanish Football Style that is dynamic and unpredictable
characterized by small pelota touches in small spaces, and hard to reason about
passes.

![TikiTaka](https://j.gifs.com/vV0MbG.gif)

### Basic Terminology
- The whole process of using Tiki Taka is called a "play"
- By "ball" we mean data
- By "pass" we mean passing ball down a path (directory) and to stop at the intended location (file)
- By "blindPass" we mean pass without looking to see if the recipient (file) is there (only do this if confident)
- By "defender" we mean the file guard that prevents us from overwriting it
- By "chipPass" we mean "pass over" or "write over" the defender while checking to see if the file exists
- By "rabona" is a blind chip pass, we mean "pass over" or "write over" the defender without checking to see if the file exists (only do this if really confident)
- By "touch" we mean setting up a location for the ball to stop at (file location)
- By "touch touch" we mean take an extra touch to create the path for the play, and then its location
- By "fake pass" we mean take the file data, put into buffer, delete the origin
- By "dribble" we mean to set up a "read stream"
- By "dribbleLongPass" we mean to set up a "read stream to write stream"
- By "shoot" we mean to set up a socket or ipc for the data to shoot through
- By "goal" it means we've succeeded on the difficult shot
