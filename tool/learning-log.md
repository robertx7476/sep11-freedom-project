# Tool Learning Log

## Tool: **Phaser**

## Project: **Gardening**

### X/X/XX:
* Text
### X/X/XX:
* Text
### X/X/XX:
* Text
### 10/28/24 - 11/3/24
- So I did learn some stuff, but there's a problem which is I forgot to link the video on the tutorial I was following so I need to find it.
- But still learned some things about impact js.
- `var someImage = new ig.Image( 'media/some-image.png' );` is to add/load in an image
- `var someSound = new ig.Sound( 'media/some-sound.*' );` is to add sounds into the game
- `var someAnimSheet = new ig.AnimationSheet( 'media/some-image.png', 8, 8 );` is something I already learned before which is to help animate/load in the animated sprite/object.
```
MyGame = ig.Game.extend({
    titleImage: new ig.Image( 'media/title.png' ),

    init: function() {
        this.backgroundImage = new ig.Image( 'media/background.png' );
    }
});
```
So inside the function, the image won't be preloaded and the titleImage will be preloaded.
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

<!--
* Links you used today (websites, videos, etc)
* Things you tried, progress you made, etc
* Challenges, a-ha moments, etc
* Questions you still have
* What you're going to try next
-->
