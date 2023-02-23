import turtle
screen = turtle.Screen()
  #set size:
screen.setup(width = 1.0, height = 1.0)
  #remove close,minimaze,maximaze buttons:
canvas = screen.getcanvas()
root = canvas.winfo_toplevel()
root.overrideredirect(1)
tracer_speed = 0
turtle.tracer(tracer_speed, 0)
turtle.hideturtle()
colour_counter = 0
counter = 0
periodic = 1 #
from datetime import datetime #create a random initiate based on the current time second
myobj = datetime.now()
random_initiator = myobj.microsecond * myobj.second * myobj.minute * myobj.hour / (1000000 * 60 * 60 * 24) * 360

def koch_curve(t, iterations, length, shortening_factor, angle):
    if iterations == 0:
        t.forward(length)          
    else:
        iterations = iterations - 1
        length = length / shortening_factor
        koch_curve(t, iterations, length, shortening_factor, angle * 1.1)
        t.left(angle * 1 + interest_number)
        koch_curve(t, iterations, length, shortening_factor, angle)
        t.right(angle * 2.4 + random_initiator + (interest_number*1.0005) + periodic*10.17238) # change this number for interest eg 2.7
        koch_curve(t, iterations, length, shortening_factor, angle)
        t.left(angle * 0.9 - (interest_number/1000) + periodic*1.17238)
        koch_curve(t, iterations, length, shortening_factor, angle)
t = turtle.Turtle()
turtle.hideturtle()
turtle.speed(10)
turtle.delay(0)



for q in range(11800000000000):
    turtle.hideturtle()
    periodic = q
    overall_size = 250
    range_setter = 15 # RANGE    
    for z in range(1):
        interest_number = 0
        extra_angle = 0.05
        t = turtle.Turtle()
        turtle.hideturtle()
        turtle.speed(3)
        turtle.delay(0)
        turtle.tracer(tracer_speed, 0)
        size_setter = 0.3
        the_shade = [q%69+10+int(random_initiator/36), q%13+20+int(random_initiator/36), q%13+20+int(random_initiator/36)] # START COLOUR
        top_shades = [80, 25, 90] # max shade out of 99 max
        add_shades = [2, 0, 3]   # rate of colour changes RGB !!!!!!!!!
        for i in range(range_setter):
          size_setter = size_setter + 0.1
          t.left(-70 - extra_angle)
          for c in range(0,3):
              if (the_shade[c] < (top_shades[c] - add_shades [c])):
                  the_shade[c] = the_shade[c] + add_shades[c] # SHADING
              else:
                  if (c == 0): the_shade[c] = (the_shade[c] - top_shades[c]) + q%69+10   #R returns
                  elif(c == 1): the_shade[c] = (the_shade[c] - top_shades[c]) + q%13+10   #G returns
                  else: the_shade[c] = (the_shade[c] - top_shades[c]) + q%13+20            #B returns
          t.color('#500000', '#' + str(the_shade[0]) + str(the_shade[1]) + str(the_shade[2])) # COLOUR
          for i in range(1): # range dictates how long it carries on
            t.begin_fill()  # COLOUR
            koch_curve(t, 4, 50 * size_setter * overall_size, 3, 60) # second number = size
            t.right(1) # don't know what this number does, started at 12, 1 is different
            extra_angle = extra_angle * 0.6 + 0.8 + (extra_angle*extra_angle)/50
            t.end_fill()  # COLOUR
            interest_number = interest_number + 0.03
        #turtle.getcanvas().postscript(file=(str(periodic+1) + ".eps")) #SAVE eps
        turtle.Screen().clear()
        turtle.reset()
        turtle.hideturtle()
        if tracer_speed < 8:
            tracer_speed = tracer_speed + 4
   

turtle.mainloop()
