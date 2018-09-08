# Making Ubuntu Chinese-Friendly!

### Chinese Pinyin Input

If you simply take a fresh install of Ubuntu and try to enable Chinese input, it won't do anything.  The solution is [here](https://askubuntu.com/questions/455682/14-04-chinese-ibus-input-no-options).

First, install the package `ibus-sunpinyin` (you can try `ibus-pinyin` but I found it annoying to use):

```
sudo apt install ibus-sunpinyin
ibus restart
```

Then go to `System Settings` -> `Language Support` and install Chinese.  You need to logout and login for the changes to take effect.

Finally, in `System Settings` -> `Text Entry`, you should be able to add `Chinese (SunPinyin) (IBus)`.

### Font Rendering

Test characters: 系，将，外，深，腿，浅，亲

Now you may notice some characters being rendered strangely (by default they may be rendered as Japanese rather than Chinese characters).  [This](https://chinese.stackexchange.com/questions/30935/chinese-font-some-characters-rendered-strangely-%E5%A4%96-%E5%B0%86/30939#30939) post outlines the issue and how to solve it.
