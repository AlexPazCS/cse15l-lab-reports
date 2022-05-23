# Lab Report Week 8
## Repository Links
[My Repository](https://github.com/AlexPazCS/markdown-parser)
[Week 7 Lab Shared Repository](https://github.com/FishInAZ/makrdown-parse-own)

## My Implementation Errors
![image](https://user-images.githubusercontent.com/103294574/169741563-869f9e1c-c290-4dfc-9f2d-0cc5fe03f7e0.png)
![image](https://user-images.githubusercontent.com/103294574/169741603-ce7c859c-6d39-4cf7-a1ae-b794c710ca05.png)
![image](https://user-images.githubusercontent.com/103294574/169741634-6528486c-9419-455d-b290-1fd4fff50fdc.png)

## Shared Implementation Errors
![image](https://user-images.githubusercontent.com/103294574/169741678-7445fdb2-b6ba-4987-8886-8b6d152951d3.png)
![image](https://user-images.githubusercontent.com/103294574/169741705-9f4641ce-37f9-4857-8efb-e3bec84f7e80.png)
![image](https://user-images.githubusercontent.com/103294574/169741845-53bbd97e-addf-4ebe-b26c-0451dbca1049.png)

## Code Reviews
1. To implement changes in the code to account for "`" in brackets and links, it would require many lines of code. As "`" <br>
may make brackets void, so many lines will be needed to account for "`" that null brackets deep in a file and go back to the <br>
original line of the file. <br>
<br>
2. To implement changes in the code to account for nested brackets and parenthesis, a great many lines of code will be required <br>
as many checks will have to occur for all brackets and parenthesis. Furthermore, the order of the nest will need to be implemented <br>
adding even more lines of code for implementation. However, implementing the escaped bracket is as simple as checking for an accompying <br>
"\" before the bracket. <br>
<br>
3. To implement changes in the code to account for new lines and line breaks, few code will be needed as the solution is adding <br>
considerations for lines in the code. This can be done and fix all possible issues for line breaks in the code. <br> 
More code maybe necessary for line breaks, but it is not too much of an issue. <br>
