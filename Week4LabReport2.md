# Week 4 Lab Report 2

#### Three code changes that were made in Lab 3

- ![Image](https://cdn.discordapp.com/attachments/852041958067273761/967897825650298900/unknown.png)
  - [Link to Failure Inducing File](https://raw.githubusercontent.com/ozheng7/markdown-parser/a895b0db7147c2f8786d2d1173145e0f79477277/test-file.md) 
  - This file was changed so that it would be able to find links even with empty lines in the file
    - empty lines previously caused the program to loop infinitly
    - ![Image](https://cdn.discordapp.com/attachments/852041958067273761/967902781774114916/unknown.png)
  - The loop was caused by the file constantly looping back to the previous parenthesis. That is why there are two numbers repeating constantly becuase it is jumping between those two. The loop was fixed by checking if the file we were checking had reached the end of the string. Once it did, it would return and end the method.

- ![Image](https://cdn.discordapp.com/attachments/852041958067273761/967906380184944651/unknown.png)
  - [Link to Failure Inducing File](https://raw.githubusercontent.com/ozheng7/markdown-parser/main/part5-secondfile.md)
  - This file was changed so that it would be able to recognize and ignore Image links
    - ![Image](https://cdn.discordapp.com/attachments/852041958067273761/967907301568700417/unknown.png)
  - The failure was caused by the program only looking for brackets, which both the links and images share. Imstead, it was changed to look for brackets and also if there is an exclamation mark in front of them, the indication for an image.

- ![Image](
- ![image](https://user-images.githubusercontent.com/103291913/164999302-c00fec6a-ba2f-4ec5-bdc0-c870af6ab0b9.png)
