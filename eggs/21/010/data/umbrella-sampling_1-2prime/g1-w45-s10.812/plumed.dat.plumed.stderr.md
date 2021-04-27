**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w45-s10.812/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:706, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: HILLS RESTART HEIGHT 0.000 W_STRIDE 50
Maybe a missing space or a typo?
[fv-az99-305:09499] *** Process received signal ***
[fv-az99-305:09499] Signal: Aborted (6)
[fv-az99-305:09499] Signal code:  (-6)
[fv-az99-305:09499] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f882d835210]
[fv-az99-305:09499] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f882d83518b]
[fv-az99-305:09499] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f882d814859]
[fv-az99-305:09499] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f882da9c951]
[fv-az99-305:09499] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f882daa847c]
[fv-az99-305:09499] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f882daa84e7]
[fv-az99-305:09499] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f882daa8799]
[fv-az99-305:09499] [ 7] plumed(+0xf47d)[0x563f9490947d]
[fv-az99-305:09499] [ 8] plumed(+0x14004)[0x563f9490e004]
[fv-az99-305:09499] [ 9] plumed(+0xf698)[0x563f94909698]
[fv-az99-305:09499] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f882d8160b3]
[fv-az99-305:09499] [11] plumed(+0xf76e)[0x563f9490976e]
[fv-az99-305:09499] *** End of error message ***
</pre>
{% endraw %}
