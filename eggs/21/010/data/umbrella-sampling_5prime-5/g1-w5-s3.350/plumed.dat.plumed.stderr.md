**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_5prime-5/g1-w5-s3.350/plumed.dat   
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
[fv-az99-305:16218] *** Process received signal ***
[fv-az99-305:16218] Signal: Aborted (6)
[fv-az99-305:16218] Signal code:  (-6)
[fv-az99-305:16218] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f618c158210]
[fv-az99-305:16218] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f618c15818b]
[fv-az99-305:16218] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f618c137859]
[fv-az99-305:16218] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f618c3bf951]
[fv-az99-305:16218] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f618c3cb47c]
[fv-az99-305:16218] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f618c3cb4e7]
[fv-az99-305:16218] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f618c3cb799]
[fv-az99-305:16218] [ 7] plumed(+0xf47d)[0x555ca3e9e47d]
[fv-az99-305:16218] [ 8] plumed(+0x14004)[0x555ca3ea3004]
[fv-az99-305:16218] [ 9] plumed(+0xf698)[0x555ca3e9e698]
[fv-az99-305:16218] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f618c1390b3]
[fv-az99-305:16218] [11] plumed(+0xf76e)[0x555ca3e9e76e]
[fv-az99-305:16218] *** End of error message ***
</pre>
{% endraw %}
