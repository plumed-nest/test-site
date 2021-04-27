**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_2prime-2/g4-w1-s8.900/plumed.dat   
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
[fv-az99-305:11650] *** Process received signal ***
[fv-az99-305:11650] Signal: Aborted (6)
[fv-az99-305:11650] Signal code:  (-6)
[fv-az99-305:11650] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f701eba1210]
[fv-az99-305:11650] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f701eba118b]
[fv-az99-305:11650] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f701eb80859]
[fv-az99-305:11650] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f701ee08951]
[fv-az99-305:11650] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f701ee1447c]
[fv-az99-305:11650] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f701ee144e7]
[fv-az99-305:11650] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f701ee14799]
[fv-az99-305:11650] [ 7] plumed(+0xf47d)[0x55e3bca7647d]
[fv-az99-305:11650] [ 8] plumed(+0x14004)[0x55e3bca7b004]
[fv-az99-305:11650] [ 9] plumed(+0xf698)[0x55e3bca76698]
[fv-az99-305:11650] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f701eb820b3]
[fv-az99-305:11650] [11] plumed(+0xf76e)[0x55e3bca7676e]
[fv-az99-305:11650] *** End of error message ***
</pre>
{% endraw %}
