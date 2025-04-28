# Entry 5
##### 4/21/25-4/27/25

### Content
My partners and I did some work on our freedom project and we created an mvp. Now we are starting to go beyond that and add edits to our project. Over the spring break, we started to create our mvp, we decided that Caron was making a title screen for our game that'll display instructions. Kiara and I started on the game itself, we created a mini game that is our MVP, we coded in falling circles, a basket that can move and interact with the falling circles, displaying the score, and stopping that game if the user collected the wrong type of circle. Kiara added animation to our game's background which makes it look cool, it is a large piece of wood moving.
### MVP
The code for the mini-game on P5js.
```
        let setting;
        let settingY = 0;
        let basket;
        let shapes;
        let score = 0;
        let gameOver = false;
        function preload() {
            setting = loadImage("wood.png");
        }
        function setup() {
            createCanvas(600, 400);
            basket = new Sprite(300, 370, 100, 20, 'static');
            basket.color = 'brown';
            shapes = new Group();
            textSize(20);
        }
        function draw() {
            background(240);
            image(setting, 0, settingY, width, height);
            image(setting, 0, settingY + height, width, height);
            settingY--;
            if (settingY < -height) settingY = 0;
            if (gameOver) {
                fill(255, 0, 0);
                textAlign(CENTER, CENTER);
                textSize(40);
                text("GAME OVER", width / 2, height / 2);
                return;
            }
            basket.x = constrain(mouseX, 50, 550);
            if (frameCount % 30 === 0) {
                let shape = new Sprite(shapes);
                shape.x = random(50, 550);
                shape.y = -20;
                shape.diameter = random(20, 40);
                shape.vel.y = random(2, 5);
                if (random() < 0.3) {
                    shape.color = 'orange';   // deadly
                    shape.isDeadly = true;
                } else {
                    shape.color = 'green';    // safe
                    shape.isDeadly = false;
                }
            }
            for (let shape of shapes) {
                if (shape.overlapping(basket)) {
                    if (shape.isDeadly) {
                        gameOver = true;
                    } else {
                        score++;
                    }
                    shape.remove();
                } else if (shape.y > height + 30) {
                    shape.remove();
                }
            }
            fill(0);
            text("Score: " + score, 10, 20);
        }
```
This is the final code for our mini game, it works decently but we are going beyond mvp so we already know what improvements we want to add to this. In the game right now, there are two different colored circles, the green ones are safe to collet and orange ones are deadly. We are going to replace the colored circles with fruits and trashbags. So, later we are going to add those pngs into the game and replace the colored circles. We are also thinking of increasing the starting speed of the falling objects.
### Engineering Design Process
We are creating our project right now and testing out it. We are at steps 5 & 6 because we are creating and editing our project. We are creating our mini game so that it can be good, and we are going to add the menu and a way to exit the mini-game to sell the fruits. We are constantly testing our code because we need to see if there are any errors.
### Skills
#### Problem decomposition
Problem decomposition is one of the skills that my partner and I have been practing a lot when we are making the mvp. As we were writing and testing our code, we kept seeing that we are getting errors. So we worked together and asked for help to overcome and fix those errors. And we fixed, I believe, all the errors. Also nefore when we were fixing errors, we were creating new errors sometimes.
#### Communication
Communication is a skill that we are also improving on, because we somewhat communicate during school, whenever we have the same periods together, and during the spring break we were communicating better. We called each other and worked on the code together, and talked to each other while coding.

[Previous](entry04.md) | [Next](entry06.md)

[Home](../README.md)
