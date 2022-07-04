# Find the most common IP Address using panda moudel
# use high-performance data structures and data analysis tools
import pandas as pd 
# The time module use to suspend execution of the calling thread for however many seconds you specify
from time import sleep 
#The Counter holds the data in an unordered collection, It allows you to count the items in an iterable list.
from collections import Counter 
# menu function created to display the menu selection 
def menu(): 
    print("=================================")
    print("Insert 1 to analyse log file")
    print("Insert 0 to quit")
    print("================================")
    return input(str(" Please select an option: "))
    sleep(1)
# this function will make run the analyser script.    
def analyse_log():
# lets you test a block of code for errors.
        try: 
# The variable logfile has been create to give an imput to insert the file on pandas module
            logfile=input("Please enter a file name you want to analise") 
            sleep(1)
# that pandas module is used to read the file log to examinate
            df = pd.read_csv(logfile, sep=' ', header=None)
            df
# The Python tr except statement catches an exception
        except FileNotFoundError:
            print("The file insert doesn't Exist")
            sleep(2)

        else:
# I variable i and module panda and 0 that is the menu head row where I can see the IP address to analyses.
            i=(df[0]) 
# I rename the variable i in a
            a=i 
# I created the variable c and I use the module counter hat will help find the most common IP and how manytimes 
            c = Counter(a) 
# This will print the most common used IP address and many times are displayed.
            print("Most frequent IP address in this file is:",c.most_common(1),"Times") 
            sleep(3)
# Set choice to be empty and display title
choice = ''
#displey menu script 
print("***Welcome to Script Analyses***")
sleep(1)
#while true used to run a loop of the menu script
while choice != '0':
# this is a combination of choice and the function menu to displey the selection of menu
    choice = menu() 


    if choice == '1':
#function to run the script 
        analyse_log() 

    elif choice == '0': 
# print Exit        
        print("Bye Bye!!!") 
        break

    else:
# print try again if there is an error on the menu and repeat on loop
        print("Try Again!") 
        sleep(2)
