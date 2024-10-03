## Assignment 1

I successfully completed Python Assignment-1 on Strings using some logics and Built-in methods.

Problem 1 :- Write a Python program to count the number of characters in a string without using len function.

    to solve the above problem i used "for loop" to iterate the given sting and updated the "c" value with adding "1" at each iteration. initially c = 0 .

Problem 2 :- Write a Python program to reverse a string without using [::-1]

    to solve the above problem i used for loop to iterate given    string with the basis of index
            i.e :- for i in range(len(string)) :
    len() -> returns the no.of characters present in the given string.
    i used "  rev += st[(len(st)-1)-i]  " logic to add the chars of given string in reverse order to the new string "rev".

Problem 3 :- Write a Python program to check if a string is a palindrome don't use [::-1].
    
    i applied same process and logic which is used in Problem 2 to get reversed string.
    to print palindrome or not.i used if-else condition.
        condition -> if the given string is equal to its reversed string then, it is called as Palindrome.

Problem 4 :- Write a Python program to find the most common character in a string.

    to solve this problem i used 
    count() function -> it returns the count of specified character in the given string.
    initially, we need to take the count of first char of the given string.  i.e max_coun = st.count(st[0])
    after that we use for loop to iterate chars and than we count the no.of occurrences of every char of the given string.
            for i in st :
                if st.count(i) > max_coun :
                    max_coun = st.count(i)
    from above code we are counting every char and checking which is greater than max_coun.if a char has more count value than max_coun then the max_coun will be updated with that perticular chars count.

Problem 5 :- Write a Python program to check if two strings are anagrams.

    we have different approaches to solve this problem.

    generally, An anagram is a word or phrase formed by rearranging the letters of another word or phrase, using all the original letters exactly once.

    we can simply solve this problem with using sorted() and comparission operator.
    if sorted(st1) == sorted(st2) :
        print("Both the Words are anagrams")
    else :
        print("Both the Words are not anagrams")
    
    But, i used another approach.

Problem 6 :- Write a Python program to remove all the vowels from a string.

    we can solve this problem with checking every char of the given string present or not in vowels < aeiouAEIOU >
    Condition -> if the char is in vowels then print that character.

Problem 7 :- Write a Python program to find the longest word in a string.

    we can solve this problem by splitting the string into a list and iterate.then, we can find the length of each word.so,we can easily find the longest word from the given string.

Problem 8 :- Write a Python program to capitalize the first letter of each word in a string [dont use built-in-function called title].

    we can solve this problem by splitting the given string into a list of elements. after that we need to iterate the list and update the first char of every word into uppercase using upper() function.
    finally we can the list into string using < .join() > function.

Problem 9 :- Write a Python program to find the frequency of each character in a string.OutPut should be in a form of Key:value pair.

    we know Dictionary can not accept repeated Keys.
    so,we can iterate the given string and count the frecuency of every char.
    then we can add char as a key and frequency a value to the dictionary

Problem 10 :- write a python programme to find the sum of all the even characters based on Ascii values.

    to get ascii value we have a built-in function ord().

    We can iterate through the string and find the ASCII value of each character. After that, we can check whether the value is even or odd. If it is even, we can update the initial variable by adding that ASCII value.
