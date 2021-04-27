**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_4-5prime/g1-w30-s6.374/plumed.dat   
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
[fv-az99-305:13348] *** Process received signal ***
[fv-az99-305:13348] Signal: Aborted (6)
[fv-az99-305:13348] Signal code:  (-6)
[fv-az99-305:13348] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f0b8a802210]
[fv-az99-305:13348] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f0b8a80218b]
[fv-az99-305:13348] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f0b8a7e1859]
[fv-az99-305:13348] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f0b8aa69951]
[fv-az99-305:13348] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f0b8aa7547c]
[fv-az99-305:13348] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f0b8aa754e7]
[fv-az99-305:13348] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f0b8aa75799]
[fv-az99-305:13348] [ 7] plumed(+0xf47d)[0x5586c3e5847d]
[fv-az99-305:13348] [ 8] plumed(+0x14004)[0x5586c3e5d004]
[fv-az99-305:13348] [ 9] plumed(+0xf698)[0x5586c3e58698]
[fv-az99-305:13348] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f0b8a7e30b3]
[fv-az99-305:13348] [11] plumed(+0xf76e)[0x5586c3e5876e]
[fv-az99-305:13348] *** End of error message ***
</pre>
{% endraw %}
