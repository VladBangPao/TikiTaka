# TikiTaka
WARNINGS: 
1. Please do not invest time in the names of these functions yet, as they are subject to change. Its too early. It's just to give you an idea.
2. TikiTaka takes an "Offensive Programming" style. Meaning, a lot of safeguards are removed in an otherwise defensive programming world. This also means we don't return feedback from functions to let you know if your move succeeds. This is designed to enforce player performance and sport like behavior.
3. TikiTaka is a sport first and foremost. However, we think (with time) you might end up more productive when you get really good at it.


## Playing Spanish Futbol with Files and Data
- Tiki Taka is a Spanish Football Style that is dynamic and unpredictable
characterized by small pelota touches in small spaces, with hard to reason about
passes.

![TikiTaka](https://media.balls.ie/uploads/2013/09/barcatikitaka.gif)

Or

![TikiTaka1](https://github.com/ItsZeusBro/TikiTaka/blob/7ac57e42d912adeb70d8160b4dea3887d6b46c16/Gifs/TikiTaka.gif)

## File Operation Function Primitives:
| Function           | params                                                                  | returns        | explanation                                                                                    |
|--------------------|-------------------------------------------------------------------------|----------------|------------------------------------------------------------------------------------------------|
| mkdir(...paths)    | takes n number of path arguments of type string                         | null           | creates empty directories with names specified in variadic arguments                           |
| create(...paths)   | takes n number of path arguments of type string                         | null           | creates empty files with names specified in variadic arguments                                 |
| rename(olP, newP)  | takes the old path that you wish to rename to the new path              | null           | renames a files name represented by argument a to argument b's file name                       |
| copyAppend(a, b)   | takes two paths.                                                        | null           | 'a' is read from and a copy of its data is appended to 'b'                                     |
| truncate(p, n)     | takes a path and n representing the number of bytes desired in the file | null           | truncates a file to the specified number of bytes n                                            |
| del(p)             | a path to file                                                          | null           | deletes a directory or a file of a valid path                                                  |
| write(p, data)     | takes a file path and some data you wish to write to it.                | null           | This function appends to the file by default.The file created if it doesn't exist              |
| overwrite(p, data) | takes a file path and some data you wish to write over the file         | null           | If file does not exist, this doesn't overwrite, otherwise it truncates then writes to the file |
| read(p)            | takes a file path that you want to read from                            | data from file | and reads from it                                                                              |
# Compound actions 
## (These are TikiTaka and Futbol moves, that we want to hook up to a graphical physics replay engine oneday)
I believe that using this type of scheme we would eventually see terminals with graphical replays one day (just for fun)

### One Touch:
This is when you touch the ball to set up a pass or shot. A good touch is one that results in separation from the defender, and allows for the successful delivery of a pass or shot on goal.

![oneTouch](https://github.com/ItsZeusBro/TikiTaka/blob/1403fc033a9b761058e16070c8ed324665eaf92b/Gifs/FirstTouch.gif)

### Two Touch:
Sometimes one touch is not enough to separate the defender. Two good touches should be enough.

![twoTouch](https://github.com/ItsZeusBro/TikiTaka/blob/1403fc033a9b761058e16070c8ed324665eaf92b/Gifs/doubleTouch.gif)

### Passare

This is a standard pass. It requires that the player with the ball successfully kicks the ball in the direction of the intended recipient and that the recipient successfully receives the ball in stride so they can do something with it.

![passare](https://github.com/ItsZeusBro/TikiTaka/blob/1403fc033a9b761058e16070c8ed324665eaf92b/Gifs/Passare.gif)

### Passagio Inverso
This is a backwards pass or shot. This can be done when the recipient (or goal) is behind you, or when the recipient will be behind you when the ball reaches the intended position.

![passareInverso](https://github.com/ItsZeusBro/TikiTaka/blob/1403fc033a9b761058e16070c8ed324665eaf92b/Gifs/BackPass.gif)

### HoherTritt
This is a high cross pass. A high cross is a pass that is lifted up in the air over defenders to reach the intended recipient in stride (typically while on their way towards the net, but not always). This is not the same as a chip pass, even though they can achieve the same result. 

![highcross](https://github.com/ItsZeusBro/TikiTaka/blob/1403fc033a9b761058e16070c8ed324665eaf92b/Gifs/highCross.gif)

### NiedrigerTritt
This is a low cross pass. A low cross is a pass that skips slightly above the ground with a large amount of force and speed. This is a good pass when the opportunity presents itself because it catches defenders off guard when they expect a high cross.

![lowcross](https://github.com/ItsZeusBro/TikiTaka/blob/1403fc033a9b761058e16070c8ed324665eaf92b/Gifs/lowcross.gif)

### No Looker
A no look pass (or shot) is as it sounds. You fool defenders by looking one way and passing (or shooting) the ball the other way. This is typically done as a ground pass or shot. (Sometimes as a no look chip pass or shot)

![nolook](https://github.com/ItsZeusBro/TikiTaka/blob/1403fc033a9b761058e16070c8ed324665eaf92b/Gifs/blindpass.gif)

### Butt Pass
This is a butt pass or shot. While you are turned from the ball and the ball is coming at you with speed (waist high), you can thrust your tuchus into the ball and deliver an unexpected pass or shot. 

![butter](https://github.com/ItsZeusBro/TikiTaka/blob/1403fc033a9b761058e16070c8ed324665eaf92b/Gifs/buttpass.gif)

### Chapeu
This is a chip pass or shot. Typically you would do this to lift the ball off the ground at short distances to keep defenders from being able to intercept the pass with a high kick. If it's a shot on goal, it is used to take advantage of an aggressive goal keeper that charges the ball carrier.

![chip](https://github.com/ItsZeusBro/TikiTaka/blob/1403fc033a9b761058e16070c8ed324665eaf92b/Gifs/chip.gif)

### Chapeu Inverso
A reverse chip requires you to have the ball elevated enough to chip it over or around defenders (as a pass or shot).

![reverseChip](https://github.com/ItsZeusBro/TikiTaka/blob/1403fc033a9b761058e16070c8ed324665eaf92b/Gifs/chippass.gif)

### Rabona
A rabona is a difficult pass or shot done while wrapping your strong foot behind your week foot to meet the ball with sufficient power to deliver a good pass or shot.

![rabona](https://github.com/ItsZeusBro/TikiTaka/blob/1403fc033a9b761058e16070c8ed324665eaf92b/Gifs/Rabona.gif)

### Bicicleta
This is mostly used as a shot, but can be used as a pass. It is when your back is turned to the intended recipient or goal. You jump, lifting your leg above your head to meet the ball at an apex that provides an optimal lift trajectory for the ball.

![bicycle](https://github.com/ItsZeusBro/TikiTaka/blob/1403fc033a9b761058e16070c8ed324665eaf92b/Gifs/Bicicleta.gif)

### Dribble
A dribble is basically when you are running with the ball at your feet through and around defenders. The ball is typically on the ground, and requires good control skills if you are closer to the opponents goal.

![dribble](https://github.com/ItsZeusBro/TikiTaka/blob/1403fc033a9b761058e16070c8ed324665eaf92b/Gifs/dribble.gif)

### Faux
A fake pass or shot, is usually a dribble move. While the defender is anticipating your pass or shot in a given direction you can fool them by simply faking the pass or shot.

![faux](https://github.com/ItsZeusBro/TikiTaka/blob/1403fc033a9b761058e16070c8ed324665eaf92b/Gifs/Faux.gif)

### Shimmy
This is when you are typically one on one against a defender while dribbling. You shake your shoulders to throw them off balance and take advantage of a pre-mature choice by the defender.

![shimmy](https://github.com/ItsZeusBro/TikiTaka/blob/7e769a4677c977d12bb47640a158832b735ae141/Gifs/shimmy.gif)

### Leg Wiggle
This is typically while the ball is settled on the ground in front of you and you are facing a defender in close proximity. You can shake your leg in one direction or the other intending to throw the defender off balance in one direction while you take it the other direction.

![wggle](https://github.com/ItsZeusBro/TikiTaka/blob/307f62ff0e8311c8c1193946162f61c9c6482540/Gifs/wggle.gif)

### Marseille Turn
This is a move while dribbling between defenders. You place your strong foot atop the ball and roll over it while turning your body in a circular motion, only to pick up the ball with your weak foot atop the ball, rolling it across your body towards your intended direction.

![mturn](https://github.com/ItsZeusBro/TikiTaka/blob/99ddb1e40a121eeb4743fe236212a3fe972ae460/Gifs/MarseilleTurn.gif)

### Ronaldo Chop
This is an aggressive dribble technique, where your foot is placed on the inside of the ball and you whip it around the ball to the outside. At high speeds dribbling towards a defender you can throw them off balance one way or the other allowing you to make a decisive move. This effect is usually compounded with multiple chops.

![chop](https://github.com/ItsZeusBro/TikiTaka/blob/307f62ff0e8311c8c1193946162f61c9c6482540/Gifs/chop.gif)

### Nutmeg
This is a dribbling technique that is used to roll the ball in between their legs, while decisively sprinting around them. Usually it fools the defender and during that brief emotional moment of despair, you can beat their reaction to the direction of your choice.

![nutmeg](https://github.com/ItsZeusBro/TikiTaka/blob/fbd6b12b9d1310319353df4e265428c2b25e2fdf/Gifs/nutmeg.gif)

### Aurelio
This is done while a defender is standing opposite to you in a strong defensive position. You take your foot outside of the ball and push it opposite the side and wrap the ball behind your other leg and towards the original side. If done quickly you can fool the defender to one side and go the other. Because it is not a dynamic move, you need to be sure you can fool the defender. You can't readjust after deciding to perform this move. If the defender is clever, they will just steal the ball as you have no other options.

![aurelio](https://github.com/ItsZeusBro/TikiTaka/blob/fbd6b12b9d1310319353df4e265428c2b25e2fdf/Gifs/Aurelio.gif)

### Cruyff Turn
This is while your back is turned from the defender. It includes a body turn and fake shot or pass, only to wrap your foot around the outside of the ball to push it across the defender to the other side.

![cruyff](https://github.com/ItsZeusBro/TikiTaka/blob/0dc5cb094eabc46aa9467a1ea9b63c2e084736e1/Gifs/cruyff.gif)

### Elastico
This dribble is typically done in stride while approaching a defender. The player with the ball takes one touch to the outside of their body, and quickly places their shin or foot on the outside of the ball to direct it opposite the initial direction. 

![elastico](https://github.com/ItsZeusBro/TikiTaka/blob/ed1ce6bb53da55b86fc7f697240a6267dda0ce6e/Gifs/elastico.gif)

### Okocha
This move requires an outside to inside foot roll (over the ball). As the ball moves to the inside towards the weak side of the body, the same foot is used  to go on the inside to outside of the ball (around the front of the ball) This fakes out the defender by making them believe the dribbler is going the strong way, while in reality the ball is rolling to the weak side. Then the ball controller quickly proceeds to move the direction of the rolling ball.

![okocha](https://github.com/ItsZeusBro/TikiTaka/blob/3c761913ce5e4e89d6ed81f1596213583e8567e8/Gifs/okocha.gif)

### Revelino
The revelino is when you take your foot inside half of the ball and push it to the outside of your body, only to quickly take it back towards the other half of your body fooling the defender to the initial strong side of the move.

![revelino](https://github.com/ItsZeusBro/TikiTaka/blob/34cf30b12cbd01fc93bdf1e183711d687b2b0f14/Gifs/Rivelino.gif)

### Fake Pull Back
This is when the defender believes you are charging in one direction and you pull back briefly only to make them lunge towards you, then you proceed with the charge move around the defender.

![pullback](https://github.com/ItsZeusBro/TikiTaka/blob/f3e77e2bf963d95f90b0b662772cbd1ed62030c1/Gifs/pullback.gif)

### Cutback
This is one of the most basic moves in futbol, where you act as if you are going one direction and quickly cut in the other direction with the ball.

![cutback](https://github.com/ItsZeusBro/TikiTaka/blob/dbc6547af36ea989003ff07ba25f9c60caa55bd5/Gifs/cutback.gif)

### Cuauhteminha
Cuauhteminha is usually done while trying to split a double team while cornered. You grab the ball with both feet and jump between the defenders with the ball.

![cuauhteminha](https://github.com/ItsZeusBro/TikiTaka/blob/dbc6547af36ea989003ff07ba25f9c60caa55bd5/Gifs/Cuauhteminha.gif)

### Rainbow

Everyones favorite futbol move. The rainbow is known for its flare and the pot of gold at the end of it. In this case, the pot of gold is getting past the defender. Like a leprachaun, the player with the ball uses trickery. They get the defender to look where they usually should, the ball, because their instincts tell them to allways keep there eye on it. But in this case, that is why the trick works. As the defender takes a moment to look at the ball, the player setting up the play breezes past them.

![rainbow](https://github.com/ItsZeusBro/TikiTaka/blob/69eba8b4a8f187965bcef0d9e8ffc11e253ffc05/Gifs/rainbow.gif)


## In the begning it will be a productivity first tool, then a game SHOULD be made with TikiTaka:

- An ***element*** is defined as a buffer, stream, or file
- Moving data (the ball) from one element to the other with protections is a ***pass***
- Moving data (the ball) from one element to the other without protections is considered a ***shot***
- ***Bad pass or shot*** is when you lose the ball to the other team. (only if your playing against someone) 
- ***A Miss*** can be mitigated with subsequent behavior to further your objectives. It means an exception was not thrown because you knew how to use mitigators.
- A ***Dribble move*** is a filter on a buffer, before a shot or pass.
- A ***touch*** is an essential element to making sure you don't miss on the pass or the shot. 
  - Buf if you take good touches, you can set yourself up for style points on subsequent shots and passes, that come much later 
    - (which add up to moral victories and real secondary points)
- ***Vertical***  passes and shots are determined by what depth in your file tree you pass or shoot to.
- ***Horizontal*** passes (left or right) are done at the same level in your file tree. If you want to do a long cross you have to specifiy a location in your file tree that is at the same tree depth.  If you don't meet this criteria its a miss (which can be mitigated), but is not considered losing the ball. Losing the ball requires that it go out of bounds (exception), or that you are playing against someone (which is a miss against an oppnent).
