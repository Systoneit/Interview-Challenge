# Engineers and Developers Interview Challenge

------------------------------- Challenge instructions -------------------------------

Once you complete this exercise, please email the submission to joinus@systoneit.com with your name, a hyphen, the position you're interviewing for, a colon, and 'Interview Challenge Submission' for in the subject line. (e.g. 'John Public - Back-End Developer: Interview Challenge Submission').

Please if you have any questions or feedback about the test, contact Charlene Smith at c.smith@systoneit.com. We're looking for cleverness and attention to detail, not how quickly you can get it done.

Please use whichever language you're comfortable with. As a developer, you're expected to have worked with a plethora of different programming languages, so represent yourself with your strongest language choice. As long as you can provide instructions on how to execute it so we can see the results, it's fine with us.

**For this homework challenge, you have to complete enough challenges to equal a total of 10 points, how you get to 10 is entirely up to you**


> **Calendar Matching (10 points):** 

Imagine that you want to schedule a meeting of a specific duration with one of your Systone co-workers. You have access to your Systone calendar and your co-workers Systone calendar (both of which contain the entirety of your respective meetings for the day in the form of `[startTime, endTime]`), as well as both of your daily bounds (i.e., the earliest and the latest times at which you're available for meetings every day, in the form of `[earliestTime, latestTime]`).

Write a function that takes in your calendar, your daily bounds, your co-worker's calendar, your co-worker's daily bounds, and the duration of the meeting that you want to schedule, and that returns a list of all the time blocks (in the form of [`startTime, endTime`]) during which you could schedule a meeting.

Note that times will be given and should be returned in military time. For example: `1:12`, `7:02`, and `17:38`.

***Sample Input***

```
calendar1 = [['9:00, '10:30'],['12:00, '13:00'], ['16:00, '18:00']]
dailyBounds1 = [['9:00, '20:30']
calendar2 = [['10:00, '11:30'],['12:30, '14:30'], ['14:30, '15:00'], ['16:00, '17:00']]
dailyBounds2 = [['10:00, '18:30']
meetingDuration = 30
```
***Sample Output***

`[['11:30, '12:00'],['15:00, '16:00'], ['18:00, '18:30']]`

> **Water Area (5 points):** 

You are given an array of non-negative integers where each non-zero integer represents the height of a pillar of width `1`. Imagine water being poured over all the pillars; write a function that returns the surface area of the water trapped between the pillars viewed from the front. Note that spilled water should be ignored.

***Sample Input***

```
heights = [0, 8, 0, 0, 5, 0, 0, 10, 0, 0, 1, 1, 0, 3]
```
***Sample Output***

`48`

> **Four-Number Sum (5 points):** 

Write a function that takes in a non-empty array of distinct integers and an integer representing a target sum. The function should find all quadruplets in the array that sum up to the target sum and return a two-dimensional array of all these quadruplets in no particular order.

If no four numbers sum up to the target sum, the function should return an empty array.

***Sample Input***

```
array = [7, 6, 4, -1, 1, 2]
targetSum = 16
```
***Sample Output***

`[[7, 6, 4, -1], [7, 6, 1, 2]]` // the quadruplets could be ordered differently

> **Smallest Difference (3 points):** 

Write a function that takes in two non-empty arrays of integers, finds the pair of numbers (one from each array) whose absolute difference is closest to zero, and returns an array containing these two numbers, with the number from the first array in the first position.

Assume that there will only be one pair of numbers with the smallest difference.

***Sample Input***

```
arrayOne = [-1, 5, 10, 20, 28, 3]
arrayTwo = [26, 134, 135, 15, 17]
```

***Sample Output***

`[28, 26]`

> **River Sizes (3 points):** 

You're given a two-dimensional array (a matrix) of potentially unequal height and width containing only 0's and 1's. Each 0 represents land, and each 1 represents part of a river. A river consists of any number of 1's that are either horizontally or vertically adjacent (but not diagonally adjacent). The number of adjacent 1's forming a river determines its size.

Write a function that returns an array of the sizes of all rivers represented in the input matrix. The sizes don't need to be in any particular order.

***Sample Input***

```
matrix = [
[1, 0, 0, 1, 0]
[1, 0, 1, 0, 0]
[0, 0, 1, 0, 1]
[1, 0, 1, 0, 1]
[1, 0, 1, 1, 0]
]
```

***Sample Output***

`[1, 2, 2, 2, 5]` // the numbers could be ordered in any way.

> **Min Number of Coins for Change (3 points):** 

Given an array of positive integers representing coin denominations and a single non-negative integer `n` representing a target amount of money, write a function that returns the smallest number of coins needed to make change for that target amount using the given coin denominations. 

If it's impossible to make change for the target amount, return `-1`.

Note that an unlimited amount of coins is at your disposal.

***Sample Input***

```
n = 7
denoms = [1, 5, 10]
```

***Sample Output***

`3`// 2x1 + 1x5

> **Bubble Sort (1 points):** 

Write a function that takes in an array of integers and returns a sorted version of that array. Use the Bubble Sort algorithm to sort the array.

***Sample Input***

```
array = [8, 5, 2, 9, 5, 6, 3]
```

***Sample Output***

`[2, 3, 5, 5, 6, 8, 9]`

> **Caesar Cipher Encryptor (1 point):** 

Given a non-empty string of lowercase letters and a non-negative integer representing a key, write a function that returns a new string obtained by shifting every letter in the input string by `k` positions in the alphabet, where k is the key.

Note that letters should "wrap" around the alphabet; in other words, the letter `z` shifted by one returns the letter `a`.

***Sample Input***

```
string = "xyz"
key = 2
```

***Sample Output***

`"zab"`

> **Palindrome Check (1 point):** 

Write a function that takes in a non-empty string, and that returns a boolean representing whether the string is a palindrome.

A palindrome is defined as a string that's written the same forward and backward. *Note*: a single-character string is not a palindrome. 

***Sample Input***

```
string = "abcdcba"
```

***Sample Output***

`true` // it's written the same forward and backward.

> **Find Three Largest Numbers (1 point):** 

Write a function that takes in an array of integers and returns a sorted array of the three largest integers in the input array.

The function should return duplicate integers if necessary; for example, it should return `[10, 10, 12]` for an input array of `[10, 5, 9, 10, 12]`.

***Sample Input***

```
array = [141, 1, 17, -7, -17, -417, 99, 75, 541, 8,7, 7]
```

***Sample Output***

`[99, 141, 541]`

> **Extra Credit - 0 points  (we recommend this, but seriously not mandatory)** 

Submit a code sample of something you've written with an explanation of its intended use. The example should:
- Have instructions on how to execute it for us to review.
- Be written in any language. Showcase your best.
- Be no more than 1,000 lines of code.

**Mandatory Work:**

- Fork this repository
- Provide instructions on how to execute your solutions
- Provide the code that solves your solutions. Use your language of choice.(Provide information on what language used)
- Alter the README to contain the steps required to:

```
1. Run the code you created.
```

- Give our account: Systoneit access to your fork, and send us an email when you’re done using the instructions above. Feel free to ask questions as needed!

**FAQS:**

**Q:** What will you be grading me on?

**A:** Scripting/Coding skills, elegance, understanding of the technologies you use, security, documentation.


**Q:** Will I have a chance to explain my choices?

**A:** Feel free to comment your code, or put explanations in a pull request within the repo. If we proceed to a phone interview, we’ll be asking questions about why you made the choices you made.

**Q:** Why doesn't the test include XY and Z?

**A:** Dope question! PLEASE free to tell us how to make the test better. 
