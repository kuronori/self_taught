#!/usr/bin/env python3
# -*- coding: utf-8 -*-
"""
Created on Fri May  1 19:49:44 2020

@author: TakahiroKurokawa
"""

def hangman():
    import random
    number=random.randint(0,4)
    words=["gollira","lion","shark","bird","fish"]
    word=words[number]
    stages=["___________     ",
            "|               ",
            "|         |     ",
            "|         o     ",
            "|        /|\    ",
            "|        / \    ",
            "|               "
            ]
    count=0
    to_write=["_"]*len(word)
    win_or_lose=False
    word_to_list=list(word)
    print(to_write)
    while count<len(stages):
        letter=input("Answer 1 letter:")
        if letter =="quit":
            break
        if letter in word_to_list:
            index=word_to_list.index(letter)
            to_write[index]=letter
            word_to_list[index]="#"
        else:
            count+=1
        print(to_write)
        print("\n".join(stages[:count]))
        if "_" not in to_write:
            print("You win!")
            print("Answer is {}".format(word))
            win_or_lose=True
            break
    if not win_or_lose:
        print("You lose!")
        print("Collect is {}".format(word))

a=hangman()

        
        