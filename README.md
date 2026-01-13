# Program-to-Find-Distance-Between-Two-Points-in-3D-Space-Using-Class
import math

class Point3D:
    def __init__(self, x, y, z):
        self.x = x
        self.y = y
        self.z = z

    def distance(self, other):
        return math.sqrt(
            (other.x - self.x) ** 2 +
            (other.y - self.y) ** 2 +
            (other.z - self.z) ** 2
        )


# Main Program
p1 = Point3D(2, 3, 4)
p2 = Point3D(5, 7, 9)

dist = p1.distance(p2)

print("Point 1 : (", p1.x, ",", p1.y, ",", p1.z, ")")
print("Point 2 : (", p2.x, ",", p2.y, ",", p2.z, ")")
print("Distance between two points :", round(dist, 2))

Output:
Point 1 : ( 2 , 3 , 4 )
Point 2 : ( 5 , 7 , 9 )
Distance between two points : 7.07

