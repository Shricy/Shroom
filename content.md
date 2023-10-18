## Izveidot number guessing game ar Phython valodu

### Sēnes Saturs

#### 1. Speles Apraksts
Laba spēle ar vienkāršu loģiku.

#### 2. Speles logika

Dators izvēle skaitli viens 1 - 100. to liek uzminet

Spele logika ir vienkarsa 
```py
import random

repeat = True

while repeat:
    number = random.randint(1, 100)
    guess = 0
    tries = 0

    while guess != number:
        if guess > number:
            print("Too big!")
        else:
            print("Too smol!")
        
        guess = int(input("Uzmini Skaitli: "))
        tries += 1
    else:
        if tries < 4:
            print("Not bad rookie")
        elif tries < 7:
            print("U should get better")
        else:
            print(f"{tries} kinda bad")
    
    response = input("Retry y/n: ")
    if response == "y":
        repeat = True
    elif response == "n":
        repeat = False
    else:
        repeat = False
```



### 3. Spelet to
