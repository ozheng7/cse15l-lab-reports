# Week 4 Lab Report 2

#### Three code changes that were made in Lab 3

- ![Image](https://cdn.discordapp.com/attachments/852041958067273761/967897825650298900/unknown.png)
  - [Link to Failure Inducing File](https://raw.githubusercontent.com/ozheng7/markdown-parser/a895b0db7147c2f8786d2d1173145e0f79477277/test-file.md) 
  - This file was changed so that it would be able to find links even with empty lines in the file
    - empty lines previously caused the program to loop infinitly
    - ![Image](https://cdn.discordapp.com/attachments/852041958067273761/967902781774114916/unknown.png)
  - The loop was caused by the file constantly looping back to the previous parenthesis. That is why there are two numbers repeating constantly becuase it is jumping between those two. The loop was fixed by checking if the file we were checking had reached the end of the string. Once it did, it would return and end the method.
