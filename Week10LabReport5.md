# Week 10 Lab Report 5


## How I found the files that different results
- I took advantage of the script.sh file to run all of the 600+ files that the folder test-files had. I recorded the results into a txt file and used vimdiff to compare the results from both of the results. I then chose the files 14 and 194. 

## Link to the MD files
- [Test File 14](https://raw.githubusercontent.com/nidhidhamnani/markdown-parser/main/test-files/14.md)
- [Test File 194](https://raw.githubusercontent.com/nidhidhamnani/markdown-parser/main/test-files/194.md)

## For Test File 14
- For this test file, my-markdown-parser's output is correct and markdown-parser's output is incorrect. 
![image](https://user-images.githubusercontent.com/103291913/172082861-79463041-0f74-473a-b888-63f61ee8a79d.png)
- On the right is markdown-parser and on the left is my-markdown-parser
---------------------------------------
- The correct output for this file should be [] as there are no links that show when inputted to CommonMark Preview.
![image](https://user-images.githubusercontent.com/103291913/172082776-2cfbd87a-b6ff-485e-b390-9d7cba096aa1.png)
---------------------------------------
- In this case, the bug here is that for markdown-parse, the program does not take into account the outside characters. The program soley just looks for the parenthesis and links which is why it gets /foo as a link, because it was in the parenthesis after the square brackets.
![image](https://user-images.githubusercontent.com/103291913/172083879-81160e81-3427-49e5-9704-748f5c6814dc.png)
- This program should also take into account the outside characters that change the meaning of the line.

## For Test File 194
- For this test file, only markdown-parser is correct. 
![image](https://user-images.githubusercontent.com/103291913/172083052-587e7bc5-5ae5-4b6a-a702-bad3117975ec.png)
- On the right is markdown-parser and on the left is my-markdown-parser
---------------------------------------
- The correct output for this file should be [url] as that is the only link that shows in the CommonMarkPreview.
![image](https://user-images.githubusercontent.com/103291913/172083167-2f6cbd6b-0ed2-45fe-9451-07f1fc1c4c8a.png)
---------------------------------------
- In this case, the bug here is that for my-markdown-parser, the program gets confused with the extra closing parenthesis after Foo*bar. What should happen is because there is an extra closing parenthesis, the one before the actual closing parenthesis should be ignored and the extra one should be added to what the link shows as. The link should then be everything inside the parenthesis after it, up to the last closing parenthesis.
![image](https://user-images.githubusercontent.com/103291913/172083973-79e173c4-2a49-4b39-88af-6c95737d4d64.png)
- This program should be essentially be more effective in finding which brackets or parenthesis are opening or closing.
