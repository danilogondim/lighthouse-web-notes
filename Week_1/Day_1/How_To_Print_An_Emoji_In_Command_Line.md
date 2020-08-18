# How to print an emoji in Command Line

1. Go to this [Emoji List](https://unicode.org/emoji/charts/full-emoji-list.html) and find emoji to use. E.g. "Grinning Face" has UTF-16 code `U+1F600`.

2. Go to [fileformat.info](http://www.fileformat.info/info/unicode/char/search.htm) and query for `U+1F600`.

3. Click on the returned result and find the row "C/C++/Java source code"; which should show `"\uD83D\uDE00"`.

4. Use this code to include the emoji in the text you will print using the console.log command.

This tutorial was originally found on [dplatz.de - How to print Emoji characters in your Java command-line application](http://dplatz.de/blog/2019/emojis-for-java-commandline.html). The only change I made was in the last step, where it previous stated to use `System.out.println("\uD83D\uDE00")` into a Java application.