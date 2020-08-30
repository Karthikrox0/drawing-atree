# drawing-atree
My first trail of drawing a tree pattern using Python Turtle 1
#🐍python program 

import turtle
wn = turtle.Screen()
t = turtle.Turtle()
wn.bgcolor("black")
t.hideturtle()
t.color("white")
t.up()
t.goto(200,300)
t.down()
t.begin_fill()
t.fillcolor("white")
t.circle(50)
t.end_fill()
t.up()
t.goto(0,-90)
t.down()

t.fd(300)
t.back(600)
t.fd(300)
t.lt(90)
t.speed(100)
def tree(i):
	if (i<10):
		return
	else:
		t.color("white")
		t.fd(i)
		t.left(30)
		tree(3*i/4)
		t.rt(60)
		tree(3*i/4)
		t.lt(30)
		t.back(i)
		
tree(100)
t.up()
t.speed(5)
t.goto(-70,190)
t.down()
t.rt(180)#1
t.fd(200)
for i in range(3):
	t.rt(90)
	t.fd(60)
	t.rt(90)
	t.fd(13)
	
t.fd(200)
t.speed(5)
t.up()
t.speed(2)
t.fd(500)
	
