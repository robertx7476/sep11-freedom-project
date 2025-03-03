# Tool Learning Log

## Tool: **Impact**

## Project: **Gardening**

### 2/24/25-3/2/25:
- Kiara made the starting area for the gardening game.
    - She put the code to make the background in the game & added movement and the background img into the game.
    - She also setted up a bit of animation.
- Separately, I did other coding.
    - I tested how to animate jumping.
        - **animation: jump 500ms infinite**
        - which animates jumping, for 500 milliseconds or .5 of a second, which goes on forever.
    - I think Kiara is doing movement with a mouse, but I know how to make keys work like wasd or arrow keys if we wanted to switch.
        - It'll be `arrow.addEventListener("keydown",)
        - And making it for all four or eight keys.
        - `var press = "event.type == "keydown")?true:false;`
        - and connected to additional code.
    - Also saw how velocity works
        - The example given is
        ```
        if (controller.up && rectangle.jumping == false) {
            rectangle.y_velocity -= 20;
            rectangle.jumping = true;
        }
        if (controller.left) {
            rectangle.x_velocity = 0.5;
        }
        if (controller.right) {
            rectangle.x velocity += 0.5;
        }
        ```
        - Which shows the sprite sliding a little after the key is pressed.
        - The last two if statements are for when the right or left key is pressed.
        - Friction & gravity is also shown.
        ```
        rectangle.y_velocity += 1.5;
        rectangle.x += rectangle.x_velocity;
        rectangle.y += rectangle.y_velocity;
        rectangle.x_velocity *= 0.9;
        rectangle.y_velocity *= 0.9;
        ```
        - The first three are affecting the gravity of the sprite.
        - The last two are the friction being applied to the velocity when the key is being pressed.
    - These are some new stuff I learned and will probably add if we decide to do arrow keys or wasd.
    - Because I think wasd and arrow keys are going to be easier to control the sprite than the mouse dragging across the screen.
    - 
### 12/2/24-12/9/24:
- Saw a video on optimization for impact
    - there is lots for loops, strings, and return
- Another game made with Impact had
    - Friction is used, animation, and type
    - they also named some like, fireDelay, and fireRate, Invincible, and weapon.
- Also saw how the creator used strings and arrays in their code.
- I tried fixing the weltmeister, but like I wrote before, previously didn't touch it and the first tutorial didn't touch it, yet we have different results.
- The weltmeister folder has another folder with many files.
    - Like pngs that I don't use but could be useful in the future.

### 11/18/24 - 11/25/24:
- The link to the tutorial that I was using is (https.//www.youtube.com/watch?v=hMXWImAuim8)
    - I finished the tutorial
    - made ping pong with different assets.
- Though there is a problem.
    - The game broke
    - I followed tutorial exacting, but the weltmeister.html file isn't working
    - That part is different from the tutorial even though neither of us changed it.

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
