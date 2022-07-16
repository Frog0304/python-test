# python-test
school assignment
import math
height = eval(input("Enter The Height Of The Wall In Meter: "))
width = eval(input("Enter The Width Of The  Wall In Meter: "))
num_of_wall = int(input("Enter The Number Of Wall: "))
area = height * width * num_of_wall

print("The Total Area is", format(area, ',.2f') + " meter square")
print("Please Choose Type Of Tile Stated Below")
print("Small Black Granite , Medium Sunset Yellow , Large Oak Wood Effect, Extra-large White Marble")
tiles = input("Enter The Type Of Tile: ")

price_of_t1, price_of_t2, price_of_t3, price_of_t4 = 85.50, 55.00, 286.00, 290.00
t1, t2, t3, t4, = 1, 1, 1, 1    # square meter covered by each box of tile
num_box1, num_box2, num_box3, num_box4 = math.ceil(area/t1), math.ceil(area/t2), math.ceil(area/t3), math.ceil(area/t4)

if tiles == "Small Black Granite":
    print("The Total Price Is RM%.2f" % str(price_of_t1 * num_box1))
    print("Number Of Boxes Needed Are", num_box1)
    if tiles == "Medium Sunset Yellow":
        print("The Total Price Is RM%.2f" % str(price_of_t2 * num_box2))
        print("Number Of Boxes Needed Are", num_box2)
    else:
        print("Thw Total Price Is RM%.2f" % str(price_of_t3 * num_bos3))
        print("The Total Price Is RM%.3f" , num_box3)
else:
   if tiles == "Extra-large White Marble":
         print("The Total Price Is RM%.2f " % str(price_of_t4 * num_box4))
         print("Number Of Boxes Needed Are", num_box4)
   else:
         print("not in area")
