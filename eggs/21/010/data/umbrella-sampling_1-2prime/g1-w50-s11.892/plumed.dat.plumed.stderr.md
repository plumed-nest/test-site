**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w50-s11.892/plumed.dat   
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
[fv-az99-305:09646] *** Process received signal ***
[fv-az99-305:09646] Signal: Aborted (6)
[fv-az99-305:09646] Signal code:  (-6)
[fv-az99-305:09646] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f670efc6210]
[fv-az99-305:09646] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f670efc618b]
[fv-az99-305:09646] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f670efa5859]
[fv-az99-305:09646] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f670f22d951]
[fv-az99-305:09646] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f670f23947c]
[fv-az99-305:09646] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f670f2394e7]
[fv-az99-305:09646] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f670f239799]
[fv-az99-305:09646] [ 7] plumed(+0xf47d)[0x55bc4187047d]
[fv-az99-305:09646] [ 8] plumed(+0x14004)[0x55bc41875004]
[fv-az99-305:09646] [ 9] plumed(+0xf698)[0x55bc41870698]
[fv-az99-305:09646] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f670efa70b3]
[fv-az99-305:09646] [11] plumed(+0xf76e)[0x55bc4187076e]
[fv-az99-305:09646] *** End of error message ***
</pre>
{% endraw %}
