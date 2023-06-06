# Week 7 Lab report
---
## Step 4:

To log into the ieng6 account:
```
<up><up><enter>
```
As I had already used the command```ssh cs15lsp23qo@ieng6.ucsd.edu``` earlier, I though this would be the fastest way.
Then I entered my password
<img width="649" alt="image" src="https://github.com/sidhantsinghvi/cse15l-lab-reports/assets/130006438/31b7d420-c3ae-4e7e-baaa-dfab937cf1c1">
---
## Step 5:

To clone the repository and store it in the file `grader-review-sidhantsinghvi00`
```
git clone <ctrl-V> <enter>
```
<img width="538" alt="image" src="https://github.com/sidhantsinghvi/cse15l-lab-reports/assets/130006438/3a91c5ba-9b7e-4343-be0e-c1759565f213">


I had previosly copied: ```git@github.com:sidhantsinghvi03/grader-review-sidhantsinghvi03.git```. 
So, I could paste it just paste without going to github.

## Step 6

I used the up arrow key for the junit tests.
```
cd grader-review-sidhantsinghvi03
```
```
<up> <up> <up> <up> <up> <up> <up> <up> <up> <up> <up> <enter>
```
<img width="1210" alt="image" src="https://github.com/sidhantsinghvi/cse15l-lab-reports/assets/130006438/1643d6ad-ab3e-4b9f-a0d0-6c24c828cf06">

This fails:
<img width="688" alt="image" src="https://github.com/sidhantsinghvi/cse15l-lab-reports/assets/130006438/cb30b2c7-eb8e-4383-9239-32f20dcebe14">

## Step 7
To fix it, I realised that usig a code from the parent directory that is already corrected should help.
So, I ran this command to get the command using this in the directory I wanted:

```
cp ../ListExamples.java
```

`/home/linux/ieng6/cs15lwi23/cs15lwi23auc/grader-review-vaibhavmaloo03`

## Step 8
I had just run the JUnit tests two step up.
```
<up> <up> <enter>
```
This ran the same JUnit tests and ran the code. THE TESTS PASSED!! 
<img width="1156" alt="image" src="https://github.com/sidhantsinghvi/cse15l-lab-reports/assets/130006438/93e70128-f537-4e72-9689-8fbfbacb09ae">

## Step 9

```
git add
git commit -m "donee"
git push
```
git add adds changes to the staging area.
git commit -m creates a new commit with a specified commit message("donee") in one line.
git push uploads local commits to a remote repository.

## End notes
Although boring, I learned how I could skip some unwanted commands to save time.
I think I took about 60% of the time I had taken earlier:)
