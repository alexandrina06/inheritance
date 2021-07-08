# inheritance
homework
class Mammal:
    def __init__(self, eye_color):
        self.eye_color = eye_color
        

    def get_eye_color(self):
        return self.eye_color
    
    def set_eye_color(self, value):
        self.eye_color = value
        
class Dog(Mammal):
    def __init__(self, eye_color, barkFrequency):
        Mammal.__init__(self, eye_color)
        self.barkFrequency = barkFrequency
        
    def bark(self):
        return self.barkFrequency
    
class Cat(Mammal):
    def __init__(self, eye_color, meowFrequency):
        Mammal.__init__(self, eye_color)
        self.meowFrequency = meowFrequency
        
    def meow(self):
        return self.meowFrequency


        
d = Dog("green", 23)
print(d.get_eye_color(), d.bark())

c = Cat("brown", 5)
print(c.get_eye_color(), c.meow())
