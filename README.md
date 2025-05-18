# My-Greatest-Fear.md
__My greatest fear in life is being stuck in room  with a group of chimpanzees__ 

# Heading Number Two
 *My greatest fear in life is being a cave diver and then being stuck in cave you thought you could fit in without anyone knowing where you are.*


## Smaller Heading

***My greatest fear in life is falling of a very a heigh and rocky cliff.***


~I am going to crossoff this text~

 🌇🚶‍♀️👀👨‍🦲🚴👋 ➡️ 🚶‍♀️👋 🏪 🥮


## This is code in JS lanuage in open processing 

``` js
dirx1=12
diry1=10
//intial position of first circle
let x1=200
let y1= 400
let radius1=50

dirx=2
diry=3

//intial position of second circle
let x=300
let y=400
let radius=95

dirx2=8
diry2=9

/// intial position of last circle
let x2=453
let y2=125
let radius2=100

//update rect properties
dirx3=5
diry3=4
//intial position of the rect
x3=30
y3=20
w=70
h=60




function setup() {
	createCanvas(windowWidth, windowHeight);
	background(464,200,19);
	
}

function draw() {
	clear();
	
	//First circle
	circle(x1, y1, radius1);
	fill("rgb(15,191,102)");
	x1 =x1+dirx1
	y1 =y1+diry1

	//when the ball hits the bottom wall
	if (y1-radius1<=0){
		diry1=-diry1
	}
	//when the ball hits the top wall
	if (y1+radius1>=windowHeight){
		diry1=-diry1
	}
	//when the ball hits the right wall
	if (x1+radius1>=windowWidth){
		dirx1=-dirx1
	}
//when the ball hits the left wall
	if (x1-radius1<=0){
		dirx1=-dirx1
	}
	
	
//second circle
	
	circle(x, y, radius);
	fill("rgb(229,36,231)")
	
	rect(x-30,y-20,w-9,h-9,20)
	
	x =x+dirx
	y =y+diry

	//when the ball hits the bottom wall
	if (y-radius<=0){
		diry=-diry
	}
	//when the ball hits the top wall
	if (y+radius>=windowHeight){
		diry=-diry
	}
	//when the ball hits the right wall
	if (x+radius>=windowWidth){
		dirx=-dirx
	}
//when the ball hits the left wall
	if (x-radius<=0){
		dirx=-dirx
	}

	
	//last circle
	circle(x2,y2,radius2);
	fill("rgb(192,39,22)");
	
	x2 =x2+dirx2
	y2 =y2+diry2

	//when ball hits the bottom wall
	if (y2-radius2<=0){
		diry2=-diry2
	}
	//when the ball hits the top wall
	if (y2+radius2>=windowHeight){
		diry2=-diry2
	}
	//when the ball hits the right wall
	if (x2+radius2>=windowWidth){
		dirx2=-dirx2
	}
//when the ball hits the left wall
	if (x2-radius2<=0){
		dirx2=-dirx2
	}

	/// new shape-rect
	rect(x3,y3,w,h);
	fill("rgb(213,46,232)")
	
	//2 circles near the rect bottom left
	 circle(x3,y3,20)
	
	//2 circles near the rect bottom right
	circle(x3+70,y3,20)
	
	x3=x3+dirx3
	y3=y3+diry3
	
	
	///when the rect hits the right wall
	if(x3+w>=windowWidth){
		dirx3=-dirx3
	}
	
	//when the rect hits the left wall
else if(x3-w<=0){
	dirx3=0.5+dirx3
}
	//when the rect hits the bottom wall
	if(y3+h>=windowHeight){
		diry3=-diry3
	}
	// when the rect hits the top wall
else if(y3-h<=0){
	diry3=0.5+diry3
}
	
}

```
