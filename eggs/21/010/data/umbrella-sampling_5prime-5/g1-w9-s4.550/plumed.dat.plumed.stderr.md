**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_5prime-5/g1-w9-s4.550/plumed.dat   
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
[fv-az99-305:16315] *** Process received signal ***
[fv-az99-305:16315] Signal: Aborted (6)
[fv-az99-305:16315] Signal code:  (-6)
[fv-az99-305:16315] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7faf409f9210]
[fv-az99-305:16315] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7faf409f918b]
[fv-az99-305:16315] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7faf409d8859]
[fv-az99-305:16315] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7faf40c60951]
[fv-az99-305:16315] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7faf40c6c47c]
[fv-az99-305:16315] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7faf40c6c4e7]
[fv-az99-305:16315] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7faf40c6c799]
[fv-az99-305:16315] [ 7] plumed(+0xf47d)[0x55ac20c5147d]
[fv-az99-305:16315] [ 8] plumed(+0x14004)[0x55ac20c56004]
[fv-az99-305:16315] [ 9] plumed(+0xf698)[0x55ac20c51698]
[fv-az99-305:16315] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7faf409da0b3]
[fv-az99-305:16315] [11] plumed(+0xf76e)[0x55ac20c5176e]
[fv-az99-305:16315] *** End of error message ***
</pre>
{% endraw %}
