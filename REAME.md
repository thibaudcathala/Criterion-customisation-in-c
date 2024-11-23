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

## ex04 - Print test result

- Modify the message the you print after every test end to now display the test status: PASS or FAIL.

## Result example

![image](https://github.com/user-attachments/assets/f32499d0-ddc2-4960-8e91-82081511e904)

![image](https://github.com/user-attachments/assets/f07f4731-7dc0-4606-b637-9c670cbc49c5)
