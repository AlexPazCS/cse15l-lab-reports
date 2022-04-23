# Lab Report Week 4
## Error 1:
![image](https://user-images.githubusercontent.com/103294574/164879378-a7e04119-3aee-4e7b-9c8d-a0edcec78106.png)
<br>Test file with error: [test-file.md](https://github.com/AlexPazCS/markdown-parser/blob/main/test-file.md)
<br>Error message:
```
java.lang.OutOfMemoryError: Java heap space
 at java.base/java.util.Arrays.copyOfRange(Arrays.java:3822)
 at java.base/java.lang.StringLatin1.newString(StringLatin1.java:769)
 at java.base/java.lang.String.substring(String.java:2709)
 at MarkdownParse.getLinks(MarkdownParse.java:20)
 at MarkdownParseTest.getLinks1(MarkdownParseTest.java:21)
 at java.base/jdk.internal.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
 at java.base/jdk.internal.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:77)
 at java.base/jdk.internal.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
 at java.base/java.lang.reflect.Method.invoke(Method.java:568)
 at org.junit.runners.model.FrameworkMethod$1.runReflectiveCall(FrameworkMethod.java:59)
 at org.junit.internal.runners.model.ReflectiveCallable.run(ReflectiveCallable.java:12)
 at org.junit.runners.model.FrameworkMethod.invokeExplosively(FrameworkMethod.java:56)
 at org.junit.internal.runners.statements.InvokeMethod.evaluate(InvokeMethod.java:17)
 at org.junit.runners.ParentRunner$3.evaluate(ParentRunner.java:306)
 at org.junit.runners.BlockJUnit4ClassRunner$1.evaluate(BlockJUnit4ClassRunner.java:100)
 at org.junit.runners.ParentRunner.runLeaf(ParentRunner.java:366)
 at org.junit.runners.BlockJUnit4ClassRunner.runChild(BlockJUnit4ClassRunner.java:103)
 at org.junit.runners.BlockJUnit4ClassRunner.runChild(BlockJUnit4ClassRunner.java:63)
 at org.junit.runners.ParentRunner$4.run(ParentRunner.java:331)
 at org.junit.runners.ParentRunner$1.schedule(ParentRunner.java:79)
 at org.junit.runners.ParentRunner.runChildren(ParentRunner.java:329)
 at org.junit.runners.ParentRunner.access$100(ParentRunner.java:66)
 at org.junit.runners.ParentRunner$2.evaluate(ParentRunner.java:293)
 at org.junit.runners.ParentRunner$3.evaluate(ParentRunner.java:306)
 at org.junit.runners.ParentRunner.run(ParentRunner.java:413)
 at org.eclipse.jdt.internal.junit4.runner.JUnit4TestReference.run(JUnit4TestReference.java:89)
 at org.eclipse.jdt.internal.junit.runner.TestExecution.run(TestExecution.java:40)
 at org.eclipse.jdt.internal.junit.runner.RemoteTestRunner.runTests(RemoteTestRunner.java:529)
 at org.eclipse.jdt.internal.junit.runner.RemoteTestRunner.runTests(RemoteTestRunner.java:756)
 at org.eclipse.jdt.internal.junit.runner.RemoteTestRunner.run(RemoteTestRunner.java:452)
 at org.eclipse.jdt.internal.junit.runner.RemoteTestRunner.main(RemoteTestRunner.java:210)
 ```
 <br>Error was made by an infinite loop created by a while loop that had an unchanging boolean check.
 <br>Bug was fixed by adding an if statement that breaks the while loop if there is no open brackets in the file.
 <br>like test-file.md.
## Error 2:
![image](https://user-images.githubusercontent.com/103294574/164879294-371c793c-eca7-4488-b9d1-1ce87028cf9d.png)
<br>Test file with error: [test-file3.md](https://github.com/AlexPazCS/markdown-parser/blob/main/test-file3.md)
<br>Error message:
```
java.lang.StringIndexOutOfBoundsException: begin 0, end -1, length 31
 at java.base/java.lang.String.checkBoundsBeginEnd(String.java:4601)
 at java.base/java.lang.String.substring(String.java:2704)
 at MarkdownParse.getLinks(MarkdownParse.java:23)
 at MarkdownParseTest.getLinks3(MarkdownParseTest.java:41)
 at java.base/jdk.internal.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
 at java.base/jdk.internal.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:77)
 at java.base/jdk.internal.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
 at java.base/java.lang.reflect.Method.invoke(Method.java:568)
 at org.junit.runners.model.FrameworkMethod$1.runReflectiveCall(FrameworkMethod.java:59)
 at org.junit.internal.runners.model.ReflectiveCallable.run(ReflectiveCallable.java:12)
 at org.junit.runners.model.FrameworkMethod.invokeExplosively(FrameworkMethod.java:56)
 at org.junit.internal.runners.statements.InvokeMethod.evaluate(InvokeMethod.java:17)
 at org.junit.runners.ParentRunner$3.evaluate(ParentRunner.java:306)
 at org.junit.runners.BlockJUnit4ClassRunner$1.evaluate(BlockJUnit4ClassRunner.java:100)
 at org.junit.runners.ParentRunner.runLeaf(ParentRunner.java:366)
 at org.junit.runners.BlockJUnit4ClassRunner.runChild(BlockJUnit4ClassRunner.java:103)
 at org.junit.runners.BlockJUnit4ClassRunner.runChild(BlockJUnit4ClassRunner.java:63)
 at org.junit.runners.ParentRunner$4.run(ParentRunner.java:331)
 at org.junit.runners.ParentRunner$1.schedule(ParentRunner.java:79)
 at org.junit.runners.ParentRunner.runChildren(ParentRunner.java:329)
 at org.junit.runners.ParentRunner.access$100(ParentRunner.java:66)
 at org.junit.runners.ParentRunner$2.evaluate(ParentRunner.java:293)
 at org.junit.runners.ParentRunner$3.evaluate(ParentRunner.java:306)
 at org.junit.runners.ParentRunner.run(ParentRunner.java:413)
 at org.eclipse.jdt.internal.junit4.runner.JUnit4TestReference.run(JUnit4TestReference.java:89)
 at org.eclipse.jdt.internal.junit.runner.TestExecution.run(TestExecution.java:40)
 at org.eclipse.jdt.internal.junit.runner.RemoteTestRunner.runTests(RemoteTestRunner.java:529)
 at org.eclipse.jdt.internal.junit.runner.RemoteTestRunner.runTests(RemoteTestRunner.java:756)
 at org.eclipse.jdt.internal.junit.runner.RemoteTestRunner.run(RemoteTestRunner.java:452)
 at org.eclipse.jdt.internal.junit.runner.RemoteTestRunner.main(RemoteTestRunner.java:210)
```
<br>Error caused by lack of parenthesis in test-file3.md causing the program to create invalid indexes.
<br>These invalid indexes led to an index out of bounds exception, which was fixed by having the program break
<br>break the while loop if there is no parenthesis to find the link in.
## Error 3:
![image](https://user-images.githubusercontent.com/103294574/164879234-a049a8ff-228e-40d1-95bb-9a520b7638b3.png)
<br>Test file with error: [test-file6.md](https://github.com/AlexPazCS/markdown-parser/blob/main/test-file6.md)
<br>Error message:
```
Expected [[]] but was [[page.com]]
```
<br>Issue with reading images as links.
<br>Added if statement to check for "!" before openBracket to indicate an image.
