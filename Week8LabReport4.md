# Week 8 Lab Report 4


[Link to my group's repository](https://github.com/21KennethTran/markdown-parser)

[Link to the repository that was reviewed](https://github.com/leahkuruvila/markdown-parser)

## Snippit One
- For Snippet One, the Markdown File should produce [url.com, google.com, ucsd.edu]
~~~
  `[a link`](url.com)

  [another link](`google.com)`

  [`cod[e`](google.com)

  [`code]`](ucsd.edu)
~~~

![image](https://user-images.githubusercontent.com/103291913/169670588-fffd6e07-1c37-43b4-afa8-b346443c861a.png)

- My Output
![image](https://user-images.githubusercontent.com/103291913/169670610-d1df5baa-fe4d-4912-9ec4-11c138a9c262.png)
- I do not think that there is a small snippet of code that I could change to fix this code because instead of getting the wrong links, this code did not get any links at all which means that in this file there is something that is messing with the reason why this code even gets links in the first place, basically another principle that I cannot fix with only a couple lines of code.

- Other Output
![image](https://user-images.githubusercontent.com/103291913/169670663-33f5d57d-ec7b-496c-bb3d-7a9e35ffa85f.png)
- I think that there is not a small line of code that I could change to fix this code because it seems like most of the code relies on the fact that before there is a link, there are square brackets. This would mean to fix this code, I would have to change a core principle of this code which would require rewriting more than a line of code.


-------------------------------------

## Snippet Two
- For Snippet Two, the output should be [b.com, a.com(()), example.com]
~~~
[a [nested link](a.com)](b.com)

[a nested parenthesized url](a.com(()))

[some escaped \[ brackets \]](example.com)
~~~

![image](https://user-images.githubusercontent.com/103291913/169670873-0a565721-4943-48ac-912e-a400a632021c.png)

- My Output
![image](https://user-images.githubusercontent.com/103291913/169670968-7f20d128-31c4-49dc-b5f3-8c11e8577923.png)
- There is again something in the way that makes it so that the program is not even picking up the links. I think that there is for sure more than 10 lines that would have to be rewritten or added to fix this problem..

- Other Output
![image](https://user-images.githubusercontent.com/103291913/169670899-9509d801-cab6-486d-a8ab-939b9e63c7e7.png)
- I think a couple lines could fix this problem. The problem that I am seeing is not being able to decide where is the start paren and end. I think just helping the file get a hand on where all the paren are and then finding the start and end would fix this problem.


---------------------------------

## Snippet Three
- For Snippet Three, the output should be [https://www.twitter.com, https://sites.google.com/eng.ucsd.edu/cse-15l-spring-2022/schedule, github.com, https://cse.ucsd.edu/]
~~~
[this title text is really long and takes up more than 
one line

and has some line breaks](
    https://www.twitter.com
)

[this title text is really long and takes up more than 
one line](
https://sites.google.com/eng.ucsd.edu/cse-15l-spring-2022/schedule
)


[this link doesn't have a closing parenthesis](github.com

And there's still some more text after that.

[this link doesn't have a closing parenthesis for a while](https://cse.ucsd.edu/



)

And then there's more text
~~~

![image](https://user-images.githubusercontent.com/103291913/169692314-39055be8-758b-4a46-818e-d9648c768b94.png)

- My Output
![image](https://user-images.githubusercontent.com/103291913/169692385-829d3fa9-2c8f-4a1f-925f-bc725e4a64f1.png)
- I think that a couple of lines would be able to solve this problem as what we really have to do is just fix it so that it reads links that are on the sane line, which could be easily done by just finidng whne a new line starts in the MarkdownFile.

- Other Output
![image](https://user-images.githubusercontent.com/103291913/169692458-91d0f6dc-9674-4c9e-9b87-31c0f454f871.png)
- I also think that this could be solved with a couple of lines of code since it also has about the same problem, with the program reading the links all the way down instead of stopping after the line ends.
