## Failure 1:

1. I found the error by manually checking outputs of arrays with links, and checking that test file to see if it was actually a link. I found </br>
that in [492](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/492.md) markdown does not consider the line a link. 
2. The test file that was not outputted correctly is [492](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/492.md).
3. Both implementations were wrong, as shown here (left: my-markdown-parser, right: cse15lsp22-markdown-parser). ![image](https://user-images.githubusercontent.com/103294574/172109920-6a0f620e-7fa4-4c42-8d05-4e7efab75e16.png)
the right output looks like this: <br>
![image](https://user-images.githubusercontent.com/103294574/172109453-d6ce8953-c1db-433a-90a7-b44a1a342d44.png)
4. ![image](https://user-images.githubusercontent.com/103294574/172112538-385d09d8-f7ed-439f-8a1f-33263c594184.png)
The reason My-Markdown-Parser outputs a link is because the String representinga potential link simply adds text between an open <br>
and closed parenthesis, so it does not account for "<>" symbols that cover words that are not turned into links. To fix the issue, <br>
one of the main things would be to not determine the potential link from what is inside two parenthesis, but also not include strings that <br>
are surrounded by "<>" symbols.


## Failure 2:

1. I found the error the same way as the first error, by looking at the text file with all the outputs and checking which ones <br>
had outputs with links, and checked those test file markdown previews.
2. The test file that was not correctly outputted is [491](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/491.md).
3. Both implementations were wrong again. Here were there incorrect outputs (left: my-markdown-parser, right: cse15lsp22-markdown-parser): ![image](https://user-images.githubusercontent.com/103294574/172110713-2f7ac69c-09e4-485d-bed7-26826f8e1166.png)
<br>The right output looks like this: 
<br>![image](https://user-images.githubusercontent.com/103294574/172110444-35fb644c-ebb3-48d1-9848-077335e9daa2.png)
4. ![image](https://user-images.githubusercontent.com/103294574/172113525-425d1d04-e499-42fb-b693-0071de6ec2ab.png)
The reason why My-Markdown-Parser has the incorrect output for test 491 is much like the issue in 492, but involves a lack of <br>
code that considers what makes a parenthesis valid. The code outlined determines the validity of the parenthesis, and it does not check <br>
for code enclosed by "<>" symbols. One step to fixing this issue is adding code to this if statement that checks if the program found <br>
found any "<>" symbols surrounding either parenthesis, and if it did, then return toReturn.
