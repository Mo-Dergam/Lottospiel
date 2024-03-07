# Lottospiel
def zahlen_erartten():
    from colorama import Fore 
    print(Fore.BLUE +"Wilkommen im Spiel")
    Z = 0
    print("Das Spiel wird in 5 secunden starten")
    import time
    t = 5
    F = 0
    time.sleep(t)
    Gewinnzahlen = []
    geratenen_zahlen = []
    while Z < 3:
       import random
       zufahllszahl1 = random.randint(1 , 15)
       Gewinnzahlen.append(zufahllszahl1)
       Z +=1
    while F < 3:
    
       geratene_Zahl = int(input("geben Sie einen zahl zwischen 1 und 15:"))
       if  1 <= geratene_Zahl <= 15:
         geratenen_zahlen.append(geratene_Zahl)
         F += 1 
       else:
        print("Sie müssen einen Zahl zwischen 1 und 15 ein geben")
        break
       
      
    print("Die gewinn Zahlen sind: ",Gewinnzahlen)
    print("Deine Zahlen: ",geratenen_zahlen)

    if Gewinnzahlen == geratenen_zahlen:
       print("Herzlischen Glückwünch")
    else:
       print("Game Over")
zahlen_erartten()

while True:
   E = int(input("um das program zu neuzusterten drücken Sie 1 und um das programm zu beenden drücken sie irgend ein zahl"))
   if E == 1:
    zahlen_erartten() 
   else:
    break
