[Google I/O 2016][1], 就要来了啊, 依旧啥也不会啊..  

终于找到 [`AutoCompleteTextView`][widget] 样式是不对的原因.  
之前 [`AutoCompleteTextView`][widget] 的光标一直是白色的, 我以为是 Android L 的兼容问题.  
[这个StackOverflow 回答][2] 虽然可以解决, 但是 样式还是不对, 光标宽度 不一致.  
最后蹲坑突发奇想 是不是 我们 AppCompat 的原因, 一查文档, 果不其然啊!  
还真有一个 [`AppCompatAutoCompleteTextView`][support.v7]. 换上去 立竿见影啊...  

看来 ChangeLog 还是得 多关注 [support-library][3], v22.1 加入的 貌似.  

[widget]: https://developer.android.com/reference/android/widget/AutoCompleteTextView.html
[support.v7]: https://developer.android.com/reference/android/support/v7/widget/AppCompatAutoCompleteTextView.html

[1]: https://events.google.com/io2016/
[2]: https://stackoverflow.com/questions/7238450/set-edittext-cursor-color
[3]: https://developer.android.com/topic/libraries/support-library/index.html#revisions
