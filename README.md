# Mypass Password Manager

## Overview
    This is a simple GUI password manager using Tkinter. It takes the following entries:
       - Website
        - Email/Email
       - Password
      And stores them into a JSON File as a dictionary. You can then access the dictionary using the "Search" button, which will look up all entries(key/valeus)       for the given website.

## Features

-GUI for an easy user interface

## Installation

    1. Ensure you have Python 3.8 or newer installed on your system. You can download it from [here](https://www.python.org/downloads/).

### Usage
    This program is a basic Command-Line-Interface Password manager to manage your passwords. The encryption methods that I chose to use are bcrypt(hash) as well as Fernet(key). I did this for two reasons.

    First, I didn't want to store the master password in the same file as the websites and passwords. I know that this program doesn't adhere to all of the security protocols and I am not saying that it does, it was a simple-ish in nature project that allowed me to create and learn about Object Oriented Programming, hash/salt, encryption keys and all the more.

    Second, I was having issues when using 1 fernet key and assigning it to two different files and locations - 1 for the master password and 1 for the password database. Plus, I was able to learn about the bcrypt module as well as hashes/salt.


#### Design Choices
    GUI vs CLI
    The first implementation fo this program I made using a command line interface for my CS-50 Python project file which is in reality mroe comprehensive as it has the same features as the GUI, however requires a master password to open the program on a command-line-interface, and stores everything using a fernet encryption key. I will slowly be implementing these features into this new GUI Version as well

    As the file started to grow bigger and bigger with my last implementation, I knew I wanted to have two separate files, one for the main password manager function which was a class and another which had the main content of the program. This was created using mainly Object_Oriented Programming


##### Options
The python program provides the following options:

    Website entry which contains:
      - Website
      - Username
      - Password

###### Files
    This project only requires the following files:
      - logo_icon.png
      - logo.png
      - mypass_password.py
      - mypass.py

    The program will create "passwords.json" on it's own during the first time you "add" an entry. Both the logo_icon as well as the logo are the same exact file, but I made them in to two separate files in the event that I would like to change the main logo or the icon in the future
    
###### Libraries/Modules
The following libraries/modules are required for the correct implementation and usage of this program. I included the documentation to each for your viewing pleasure:

    import os # https://docs.python.org/3/library/os.html
    import random # https://docs.python.org/3/library/random.html
    import string # https://docs.python.org/3/library/string.html
    from tkinter import * # https://docs.python.org/3/library/tk.html
    from tkinter import messagebox # https://docs.python.org/3/library/tkinter.messagebox.html

