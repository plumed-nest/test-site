**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_5prime-5/g1-w23-s8.750/plumed.dat   
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
[fv-az99-305:15971] *** Process received signal ***
[fv-az99-305:15971] Signal: Aborted (6)
[fv-az99-305:15971] Signal code:  (-6)
[fv-az99-305:15971] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f198fae1210]
[fv-az99-305:15971] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f198fae118b]
[fv-az99-305:15971] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f198fac0859]
[fv-az99-305:15971] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f198fd48951]
[fv-az99-305:15971] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f198fd5447c]
[fv-az99-305:15971] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f198fd544e7]
[fv-az99-305:15971] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f198fd54799]
[fv-az99-305:15971] [ 7] plumed(+0xf47d)[0x55c9007fa47d]
[fv-az99-305:15971] [ 8] plumed(+0x14004)[0x55c9007ff004]
[fv-az99-305:15971] [ 9] plumed(+0xf698)[0x55c9007fa698]
[fv-az99-305:15971] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f198fac20b3]
[fv-az99-305:15971] [11] plumed(+0xf76e)[0x55c9007fa76e]
[fv-az99-305:15971] *** End of error message ***
</pre>
{% endraw %}
