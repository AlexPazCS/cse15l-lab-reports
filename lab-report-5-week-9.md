## Failure 1:

1. I found the error by manually checking outputs of arrays with links, and checking that test file to see if it was actually a link. I found </br>
that in [492](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/492.md) markdown does not consider the line a link. 
2. The test file that was not outputted correctly is [492](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/492.md).
3. Both implementations were wrong, as shown here (left: my-markdown-parser, right: cse15lsp22-markdown-parser). ![image](https://user-images.githubusercontent.com/103294574/172109920-6a0f620e-7fa4-4c42-8d05-4e7efab75e16.png)
the right output looks like this: <br>
![image](https://user-images.githubusercontent.com/103294574/172109453-d6ce8953-c1db-433a-90a7-b44a1a342d44.png)
4.


## Failure 2:

1. I found the error the same way as the first error, by looking at the text file with all the outputs and checking which ones <br>
had outputs with links, and checked those test file markdown previews.
2. The test file that was not correctly outputted is [491](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/491.md).
3. Both implementations were wrong again. Here were there incorrect outputs (left: my-markdown-parser, right: cse15lsp22-markdown-parser): ![image](https://user-images.githubusercontent.com/103294574/172110713-2f7ac69c-09e4-485d-bed7-26826f8e1166.png)
<br>The right output looks like this: 
<br>![image](https://user-images.githubusercontent.com/103294574/172110444-35fb644c-ebb3-48d1-9848-077335e9daa2.png)
