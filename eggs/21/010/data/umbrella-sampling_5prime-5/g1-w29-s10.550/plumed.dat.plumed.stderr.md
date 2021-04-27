**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_5prime-5/g1-w29-s10.550/plumed.dat   
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
[fv-az99-305:16119] *** Process received signal ***
[fv-az99-305:16119] Signal: Aborted (6)
[fv-az99-305:16119] Signal code:  (-6)
[fv-az99-305:16119] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7efcef9e2210]
[fv-az99-305:16119] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7efcef9e218b]
[fv-az99-305:16119] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7efcef9c1859]
[fv-az99-305:16119] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7efcefc49951]
[fv-az99-305:16119] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7efcefc5547c]
[fv-az99-305:16119] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7efcefc554e7]
[fv-az99-305:16119] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7efcefc55799]
[fv-az99-305:16119] [ 7] plumed(+0xf47d)[0x55be89ae847d]
[fv-az99-305:16119] [ 8] plumed(+0x14004)[0x55be89aed004]
[fv-az99-305:16119] [ 9] plumed(+0xf698)[0x55be89ae8698]
[fv-az99-305:16119] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7efcef9c30b3]
[fv-az99-305:16119] [11] plumed(+0xf76e)[0x55be89ae876e]
[fv-az99-305:16119] *** End of error message ***
</pre>
{% endraw %}
