**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_2prime-2/g1-w18-s7.588/plumed.dat   
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
[fv-az99-305:11039] *** Process received signal ***
[fv-az99-305:11039] Signal: Aborted (6)
[fv-az99-305:11039] Signal code:  (-6)
[fv-az99-305:11039] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f84139ae210]
[fv-az99-305:11039] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f84139ae18b]
[fv-az99-305:11039] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f841398d859]
[fv-az99-305:11039] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f8413c15951]
[fv-az99-305:11039] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f8413c2147c]
[fv-az99-305:11039] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f8413c214e7]
[fv-az99-305:11039] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f8413c21799]
[fv-az99-305:11039] [ 7] plumed(+0xf47d)[0x55e40f95847d]
[fv-az99-305:11039] [ 8] plumed(+0x14004)[0x55e40f95d004]
[fv-az99-305:11039] [ 9] plumed(+0xf698)[0x55e40f958698]
[fv-az99-305:11039] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f841398f0b3]
[fv-az99-305:11039] [11] plumed(+0xf76e)[0x55e40f95876e]
[fv-az99-305:11039] *** End of error message ***
</pre>
{% endraw %}
