# Palindrome

### Overview
Write a platform independent C++11 application that takes a list of strings [a-z] that may or may not be re-arranged to produce a [palindrome](https://en.wikipedia.org/wiki/Palindrome) and print the corresponding palindrome to **stdout**, if applicable.

### Re-arranging
A string may or not be able to produce a palindrome by being re-arranged. For example, the string 'cqc' does not require re-arranging because it is already a palindrome, the string 'zzx' can be re-arranged to 'zxz' to produce a palindrome, and finally the string 'zwq' cannot be re-arranged in any way to produce a palindrome.

### Input
A list of strings provided by **stdin** delineated by a new-line character. The aforementioned string's characters are **ONLY** comprised of the regular expression [a-z] (sanitization is not necessary).

### Output
A list of input strings and their, if applicable, **re-arranged** palindrome result. (Said list does not have to be in the same order as the input, ex: you can use multithreading).

### Example

###### `words.txt` contents:
> racecar

> matt

> john

> x

> qqy

> att

> aallu

> ulala

> kk

###### Calling pattern
`./palindrome < words.txt`


###### Output (may be in any order)
> racecar -> racecar

> matt -> NONE

> john -> NONE

> x -> x

> qqy -> qyq

> att -> tat

> aallu -> alula

> ulala -> alula

> kk -> kk

### Evaluation Criteria

The application must be able to identify a palindrome and generate one from a string if possible. The code sample will be evaluated on code clarity, efficiency/optimization techniques, rationale, and creativity. A build system is expected, with preference for CMake or a plain Makefile.
