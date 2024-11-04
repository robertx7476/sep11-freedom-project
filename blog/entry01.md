# Entry 1
##### 10/28/24 - 11/3/24

### Content
In my first Blog, I will be explaining what tool I chose, why I chose my tool, and how I tinkered with my tool. The tool that I finalized is *Impact.js*. I choose Impact because it is a game engine and I wanted to create a gardening game with my partners. So far I did some tinkering with this tool. I tinkered by following a youtube tutorial and recreating the game pong. I did change some code up and customized it a bit. For the blocks, I put images of frying pans, and I put the ball as a soccer ball.
Learning Log:
```
### 10/21/24:
- This week I was watching a tutorial on youtube and following along
    - I made multiple new folders and downloaded files
    - The game I was recreating is pong.
    - I added my own imgs, and I followed along with the code
- So I learned
    - how to adjust size `size: (x:48,y:48),`
    - how to add keybinds into the game
```
	init: function() {
	ig.input.bind( ig.KEY.UP_ARROW, 'up' )
	ig.input.bind( ig.KEY.DOWN_ARROW, 'down' )
},
```
- And I started learning code on how to animate
```
this.addAnim('idle',0.1, [0,1,2,3,4,4,4,4,3,2,1] );
```
- the numbers in the bracket is the frames from the animSheet.
```
So I started learning how to animate. I know how to link the keyboard with keys, and I know I to change the size of things in the game.
### Sources
Before Impact, I wanted to do Phaser. But I didn't know how to do Phaser, and I can see that it will be way harder to create the game I want in Phaser compared to Impact, so I chose Impact. For Phaser, I looked at their [Introduction document](https://phaser.io/tutorials/making-your-first-phaser-3-game/part1). I read through all the documents, and it did help me learn how to make a platformer game. But since I didn't want a platformer, I wasn't super interested and I saw on [Impact](https://impactjs.com/games) that people made a lot of different types of games on there.
### EDP
I am in the researching/learning phase of the **EDP/Engineering Design Process**. Because I first had to decide what tool I wanted to use, and now I am further learning and understanding the tool.
### Skills
Organization is something I am okay at, but I did organize where my files and what I am tinkering in where it is supposed to be. I put all the files and folders under project so it is directly above my sep11-freedom-project folder.

And another skill is creativity because I was super creative/silly when tinkering. Because the images I use for the game was silly, like planning to make the pong game use a frying pan to hit a soccer ball back and forth.

[Next](entry02.md)

[Home](../README.md)
