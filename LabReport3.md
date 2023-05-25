# Week 5 Lab report
Using grep commands
## Sources:
[ChatGPT](https://chat.openai.com/chat)

## grep -c
This command searches for the given phrase and prints the number of lines with the occurence of that word.

```
grep -c "law" chapter-2.txt
5
```
So, "law" occurs five times in chapter-2.txt file.

```
grep -c "exile" chapter-2.txt
4
```
So, "exile" occurs four times in chapter-2.txt file.
## Uses
This command is commonly used to obtain a quick summary of the number of occurrences of a specific pattern within a file or a set of files.

## grep -rl
The command recursively searches for all the files that conatains the pattern and returns the name of the matching file.

```
$ grep -rl " DOJ Inspector General interview of Thomas A., May" 
chapter-13.3.txt
```
The command "grep -rl ' DOJ Inspector General...' ": goes through all files and searches for this phrase, when found, it returns the file names.

```
$ grep -rl " Bin Ladin gave a videotaped interview to ABC News "
chapter-2.txt
```
So, the line "Bin Ladin..." is only in chapter-2.txt

```
$ grep -rl " nothingnothingnothingnothingnothing "

```
This phrase is nowhere, so prints nothing .
## Uses
This command could be very useful in filtering out files that satisfy a specific requirement that the user has.

## grep -o

This command prints the exact line of that contains the pattern.
```
$ grep -o "population" chA.txt
population
population
```
The command ```grep -o "population" chA.txt``` searches for the exact word "population" in the file and prints each occurrence of it on a separate line.
This means that the file has two occurences of the phrase "population".

```
$ grep -o "bveihbrj" chA.txt

```
This prints nothing as there is no ocurrence of "bveihbrj" in the file listed.
## Uses
This could be useful when we have to focus on and extract the specific matching patterns rather than displaying the entire line containing the pattern.

## grep -A n

This command prints the searched line and and n lines after it.

```
grep -A 2 "In December 1999, NSA began placing caveats on all of its Bin Ladin reports that precluded sharing of any of the reports' contents with criminal prosecutors or FBI agents investigating criminal matters without first obtaining OIPR's permission." chapter-13.3.txt 
In December 1999, NSA began placing caveats on all of its Bin Ladin reports that
precluded sharing of any of the reports' contents with criminal prosecutors or FBI
agents investigating criminal matters without first obtaining OIPR's permission.
These caveats were initially created at the direction of Attorney General Reno and
applied solely to reports of information gathered from three specific surveillances
she had authorized. Because NSA decided it was administratively too difficult to
determine whether particular reports derived from the specific surveillances
authorized by the attorney general, NSA decided to place this caveat on all its
terrorism-related reports.
```

This prints 2 lines after the line that contains "In December 1999, NSA began...  ".

```
grep -A 4 "The next four months were spent setting up the teams in Nairobi and Dar es Salaam." chapter-2.txt 
 The next four months were spent setting up the teams in Nairobi and Dar es Salaam.
Members of the cells rented residences, and purchased bomb-making materials and
transport vehicles. At least one additional explosives expert was brought in to
assist in putting the weapons together. In Nairobi, a hotel room was rented to put
up some of the operatives. The suicide trucks were purchased shortly before the
attack date.
```
This prints 4 lines after "The next four months...".
## Uses
In summary, grep -A allows you to retrieve not only the matching lines but also a specified number of lines that follow each match, providing valuable context and making it easier to analyze and understand the surrounding information.
