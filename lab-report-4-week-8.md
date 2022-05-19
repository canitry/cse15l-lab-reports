[Link to my markdown-parse repository]()

[Link to reviewed-markdown-parse repository]()

Each snippet's expected output was decided based on the VSCode preview and how the actual markdown file was displayed in Github.

![result](lab4/withfixMain.png)

# Snippet 1:
```

```

## Test for snippet 1:
```
@Test
public void testSnippet1() throws IOException
{
    assertEquals(List.of("`google.com"), MarkdownParse.getLinks(Files.readString(Paths.get("snippet1.md"))));
}
```

## My implementation's output:

Failure. It did not recognize the difference between
![result](lab4/withfixtest1.png)

### Possible fix:

## Reviewed implementation's output:

Failure. exp...
![result]()

## Possible fix:

# Snippet 2:
```

```

## Test for snippet 2:
```
@Test
public void testSnippet2() throws IOException
{
    assertEquals(List.of("a.com", "a.com(())", "example.com"), MarkdownParse.getLinks(Files.readString(Paths.get("snippet2.md"))));
}
```

## My implementation's output:

Failure. It led to an index out of bounds error. exp...
![result](lab4/withfixtest2.png)

### Possible fix:

## Reviewed implementation's output:

Failure. exp...
![result]()

### Possible fix:

# Snippet 3:
```

```

## Test for snippet 3:
```
@Test
public void testSnippet3() throws IOException
{
    assertEquals(List.of("https://www.twitter.com", "https://sites.google.com/eng.ucsd.edu/cse-15l-spring-2022/schedu", "https://cse.ucsd.edu/"), MarkdownParse.getLinks(Files.readString(Paths.get("snippet3.md"))));
}
```

## My implementation's output:

Failure. It led to an index out of bounds error. exp...
![result](lab4/withfixtest3.png)

### Possible fix:

## Reviewed implementation's output:

Failure. exp...
![result]()

### Possible fix: