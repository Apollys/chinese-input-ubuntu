# Making Ubuntu Chinese-Friendly!

### Chinese Pinyin Input

If you simply take a fresh install of Ubuntu and try to enable Chinese input, it won't do anything.  The solution is [here](https://askubuntu.com/questions/59356/how-do-i-get-chinese-input-to-work).

First, install the package `ibus-pinyin`:

```
sudo apt install ibus-pinyin
ibus restart
```

Then go to `System Settings` -> `Language Support` and install Chinese.  You (ostensibly, I didn't check) need to logout and login for the changes to take effect.

Finally, in `System Settings` -> `Text Entry`, you should be able to add `Chinese (Pinyin) (IBus)`.

### Font Rendering

Now you may notice some characters being rendered strangely (by default they may be rendered as Japanese rather than Chinese characters).  [This](https://chinese.stackexchange.com/questions/30935/chinese-font-some-characters-rendered-strangely-%E5%A4%96-%E5%B0%86/30939#30939) post outlines the issue and how to solve it.
