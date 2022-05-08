# KerenValencia.giyhub.io
Python desde Cero
from matplotlib.font_manager import json_load
from animal import mammal
import json

class feline(mammal):
    speak: str
    def __init__(self,color):
        super().__init__(color, "feline")
        self.speak = "Miau!"

class canine(mammal):
    speak: str
    def __init__(self,color):
        super().__init__(color, "canine")
        self.speak = "Waou!"
        

dog = canine("black")
cat = feline("yellow")
dog.info()
cat.info()

list_canine = ["perro","lobo", "zorro", "chacale", "coyote", "cuone", "dingo", "licaone", "aguará" "guazú", "guará", "culpeo", "aguarachay", "culpeo" , "vulpinos"]
list_feline = ["gato","tigre", "pantera", "puma", "lince", "guepardo", "león", "jaguar"]
json_animal = json()

try:
    x = list_canine.index(input())
    y = list_feline.index(input())
    print(x)
except ValueError:
    print("No es canine")
except TypeError:
    print("TypeError")
except:
    print("Unknow Error")
