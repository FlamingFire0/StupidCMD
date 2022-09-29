#import
import os
import sys

help = "Help:\nhelp | this list\nsugus | test command\nexit | exits the program" #help | segítség szöveg


    
print("Stupid CMD uwu V1\n Made by Manel | made in China")  # start msg | szöveg
    
while True: #loop
        
    cmd = input("» ")  # input | (cmd) = input ⏎
        
    if cmd == "" or cmd.startswith(" "):  # anti empty cmd™ | ha (cmd) = "" vagy (cmd) = " " ⏎
        continue #next | kihagyni
        
    elif cmd == "help":     # help | ha (cmd) = "help" ⏎
        print(help) # msg | segítség szöveg
            
    elif cmd.startswith("calc"):    # test  | ha (cmd) kezdődik "calc" -al ⏎
        
        _calc = cmd.split()         #slice | felvágás
        
        print(eval(_calc[1]))      # msg | szöveg: számolás
        
    elif cmd == "exit":     # exit | ha (cmd) = "exit" ⏎
        
        exit()          # exit | kilépni
            
    else:  # else | ha (cmd) semmivel nem egyenlő ⏎
        
        print("Error: No Command Found: \"" + cmd + "\"")  # error | hiba
            