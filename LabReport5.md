# Week 10 Lab Report 
## Part 1 : Debugging Scenario
---
****I have used the code from week 3 to demonstrate some common issues****

---
Student:

I use a macbook, and the terminal in VS Code. After i log in ien6, I can'tcompile the files. My lab is due in an hour, pleaseee help fast

<img width="822" alt="image" src="https://github.com/sidhantsinghvi/cse15l-lab-reports/assets/130006438/74cc8501-5759-41c3-af7c-d672ae64aee2">
---
TA:

You should give more information when you ask a question. However, here I can help you as I can see the ```ls``` command you have used.
So, you're trying to compile a file that isn't even in the same directory that the system is in right now! Think of what you could do and make a reply to the post.

---

Student:

Ohhh, my bad. I get it. This is what i've done to fix the condition.:

<img width="1106" alt="image" src="https://github.com/sidhantsinghvi/cse15l-lab-reports/assets/130006438/6dcd88c3-93ff-4e58-9169-be8692cbe398">

However, help me! I'm using the same device and the terminal as before and my task is to write tests that find bugs with the code and the tests I write don't do anything!
Here are my tests and the code:

<img width="504" alt="image" src="https://github.com/sidhantsinghvi/cse15l-lab-reports/assets/130006438/84456c61-fb04-40c0-870a-1af4779e03f0">

<img width="741" alt="image" src="https://github.com/sidhantsinghvi/cse15l-lab-reports/assets/130006438/6b24554e-4049-49e6-a665-c385bfaa6677">

---
Student again:

Please I have 20 more minutes.

---

Student2:

Hold up. I see that youre trying to get edge cases ***BUT*** you need to look at the code to understand whats missing. See how the code runs, its not that hard to come up with examples.

---
TA:

Thats a well-worded answer @Student2. You haven't given much information but have given some small hints.

---
Student:

Ohh, thank you very much you're a life saver. The code was not running well for lists of length greater than one as it was losing the first element, and the reversedInPlace method was reassigning the empty array to the values This is what I did:

<img width="538" alt="image" src="https://github.com/sidhantsinghvi/cse15l-lab-reports/assets/130006438/1485df5d-bdc4-4fb1-80e2-3c4dc3adfeba">
Also, I fixed the code by assgning the first value to another method and changing the array the reversed method was using.

---
End notes:

1. I used the directory and files from lab3.
2. Full command line is shown above
3. Contents of files used:

<img width="538" alt="image" src="https://github.com/sidhantsinghvi/cse15l-lab-reports/assets/130006438/cd019312-f3bc-4c62-a181-ca62868ca3be">

<img width="538" alt="image" src="https://github.com/sidhantsinghvi/cse15l-lab-reports/assets/130006438/7ef4e6ba-9d96-4197-81d1-c2682ac3e081">

Description to fix bug is given above by the student.

***Summary***

So, I went through three bugs here.
The first one is one that confused me the most during my first couple weeks in this class. Understanding how to change the directory and when to change it is very important. So, I decided to cover that in this lab.
I felt that just one was too less, so, I added two codin bugs that were related to lists.

---

## Part 2
## Reflection

Almost everything I learned in the second half was stuff I did not know earlier. I particularly enjoyed debugging in lab 9. The features of vim, as well, I felt were pretty cool. I did not think of being able to edit files in the terminal.
Something cool i learned was that vim holds a huge potential use in CSE30, which I will be doing next quarter.
