# reloj_

y_position = 0
color_is = False
def setup():
    size(600,610)
    
def draw():
    global y_position 
    background(255)
    if color_is == True:
       fill(230, 0, 38)
    else:
       fill(0, 47, 187)

    ellipse(width /1.15, y_position, 50, 50)
    if y_position > height:
       y_position = 0
    else:
       y_position = map(second(), 0, 59, 0, height)


    ellipse(width / 5, y_position, 50, 50)
    if y_position > height:
       y_position = 0
    else:
       y_position = map(minute(), 0, 59, 0, height)
       
    ellipse(width / 1.85, y_position, 50, 50)
    if y_position > height:
       y_position = 0
    else:
       y_position = map(hour(), 0, 23, 0, height)
    line(425, 0,425, 600)
    line(225,0,225,600)
    line(25,0,25,600)
    
    line(0,150,425,150)
    line(0, 300, 425, 300)
    line(0,450,425,450)
    line(0,600,425,600)
    line(0,35,600,30)
    line(425,50,600,50)
    line(425,75,600,75)
    line(425,100,600,100)
    line(425,125,600,125)
    line(425,150,600,150)
    line(425,175,600,175)
    line(425,200,600,200)
    line(425,225,600,225)
    line(425,250,600,250)
    line(425,275,600,275)
    line(425,300,600,300)
    line(425,325,600,325)
    line(425,350,600,350)
    line(425,375,600,375)
    line(425,400,600,400)
    line(425,425,600,425)
    line(425,450,600,450)
    line(425,475,600,475)
    line(425,500,600,500)
    line(425,525,600,525)
    line(425,550,600,550)
    line(425,575,600,575)
    line(425,600,600,600)
    
    global color_is
    color_is = not color_is