# Criterion customisation in c

## Criterion documentation:
The documentation will help you to complete each task:
- Web site: https://criterion.readthedocs.io/en/stable/index.html
- PDF: [criterion-readthedocs-io-en-stable.pdf](https://github.com/user-attachments/files/17882077/criterion-readthedocs-io-en-stable.pdf)

## ex00
- Clone this repository
- Go at the root of this repository
- Create a new c filewith a name like "test_interface.c"
- Compile the given my_test.c and your test_interface.c (that is actually empty). `gcc -o my_beautiful_test my_test.c test_interface.c -lcriterion`
- Run the generated binary, it should output somthing like this:
![image](https://github.com/user-attachments/assets/9e1af1bb-0610-42c4-995d-3b8eaf6dbe31)  
You can see that criterion print a lot of thing, that the part that we will customise.
- Now run you program with as argument `--verbose=3`, it should print nothing, it's what we want, we will go from this to print our own message.

## ex01 - Print a message **before all** test start
#### https://criterion.readthedocs.io/en/stable/hooks.html

- Print a message like **`Tests Results`** before any test start. (you don't have to modify my_test.c to do this, read carefully the documentation)

Here is an **example** of result  
![image](https://github.com/user-attachments/assets/ee14fb02-ad21-4494-97ea-2efdc30dad2e)  
It can look like this, but you are totally free to print any thing that you think is revelant.

## ex02 - Print a message **after all** test end
#### https://criterion.readthedocs.io/en/stable/hooks.html

- Print a message like **`All Tests End.`** after all test end. (you don't have to modify my_test.c to do this, read carefully the documentation)

Here is an **example** of result  
![image](https://github.com/user-attachments/assets/41c00eca-ea26-4781-84aa-a163e4bee251)  
It can look like this, but you are totally free to print any thing that you think is revelant.

## ex03 - Print a message **after every** test end
#### https://criterion.readthedocs.io/en/stable/hooks.html

- Print a message like **`Test end.`** after every test end. (you don't have to modify my_test.c to do this, read carefully the documentation)

Here is an **example** of result (there is ~50-60 line, the image is cut)   
![image](https://github.com/user-attachments/assets/7e2a29a2-f07a-4f8a-826b-d16a25914394)   
It can look like this, but you are totally free to print any thing that you think is revelant.

## ex04 - Print test status
#### https://criterion.readthedocs.io/en/stable/hooks.html

- Modify the message that you print after every test end to now display the test status: PASS or FAIL. (If you don't know where to have this information: https://criterion.readthedocs.io/en/stable/hooks.html)
- You can add as mush information as you want: test duration, test name, test description, etc. Also think of what you want to print when a test fail: test file, assertion line, test that fail, test name, test description, etc.

Here is an **example** of result (the image is cut)    
![image](https://github.com/user-attachments/assets/042fe38d-af7b-4600-963a-e5f79385925d)  
It can look like this, but you are totally free to print any thing that you think is revelant.

## ex05 - Print test summary
#### https://criterion.readthedocs.io/en/stable/hooks.html

- Modify the message that you print at the end of all test to now print a summary of all test result, it can contain: number of test, number of passing test, number of failing test, etc. You can add as mush information as you want.

Here is an **example** of result (the image is cut)  
![image](https://github.com/user-attachments/assets/a7d0929b-99d1-42cf-aa86-6688477e0318)  
It can look like this, but you are totally free to print any thing that you think is revelant.

## ex06 - Print a progress bar

- At the end of all test display a progress. You can add color to the progress bar like: red if passing test is < 25%, yellow if passing test is < 75% and green if passing test is > 75%.

Here is an **example** of result (the image is cut)   
![image](https://github.com/user-attachments/assets/81aaacdd-4019-4181-aff8-a41fbc8b437c)   
It can look like this, but you are totally free to print any thing that you think is revelant.
Here is the character that I have used for the progress bar: `█` and `▒`.

## ex07/Bonus - Customise as you want

- Now that you now how to manipulate the data structure used in criterion, you are free to add as mush new feature as you want.

## End Result example

![image](https://github.com/user-attachments/assets/f32499d0-ddc2-4960-8e91-82081511e904)

![image](https://github.com/user-attachments/assets/f07f4731-7dc0-4606-b637-9c670cbc49c5)
