# CSE15L Week 5 & 6 Lab Report

## Code Snippet 1
----
![](snippet1-output.png)
<p align="center">
<em>Expected output for code snippet 1</em>
</p>

```
@Test
    public void testMarkdownParseSnippet1() throws IOException {
        Path fileName = Path.of("test-file5.md");
        String content = Files.readString(fileName);
        assertEquals("[`google.com, google.com, ucsd.edu]", MarkdownParse.getLinks(content).toString());
    } 
```
<p align="center">
<em>JUnit test for code snippet 1 in MarkdownParseTest.java</em>
</p>

The test did not pass for my implementation of MarkdownParse.java on code snippet 1

![](own-test-result-snippet1.png)
<p align="center">
<em>JUnit output for snippet 1 for my implementation</em>
</p>

## Code Snippet 2
----
![](snippet2-output.png)
<p align="center">
<em>Expected output for code snippet 2</em>
</p>

```
@Test
    public void testMarkdownParseSnippet2() throws IOException {
        Path fileName = Path.of("test-file6.md");
        String content = Files.readString(fileName);
        assertEquals("[a.com, a.com(()), example.com]", MarkdownParse.getLinks(content).toString());
    }
```
<p align="center">
<em>JUnit test for code snippet 2 in MarkdownParseTest.java</em>
</p>

![](own-test-result-snippet1.png)
<p align="center">
<em>JUnit output for snippet w for my implementation</em>
</p>



## Code Snippet 3
---
![](snippet3-output.png)
<p align="center">
<em>Expected output for code snippet 3</em>
</p>

```
@Test
    public void testMarkdownParseSnippet3() throws IOException {
        Path fileName = Path.of("test-file7.md");
        String content = Files.readString(fileName);
        assertEquals("[https://sites.google.com/eng.ucsd.edu/cse-15l-spring-2022/schedule]", MarkdownParse.getLinks(content).toString());
    } 
```

<p align="center">
<em>JUnit test for code snippet 3 in MarkdownParseTest.java</em>
</p>