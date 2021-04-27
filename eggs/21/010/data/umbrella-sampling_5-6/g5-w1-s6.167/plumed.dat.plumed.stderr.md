**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_5-6/g5-w1-s6.167/plumed.dat   
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
[fv-az99-305:15454] *** Process received signal ***
[fv-az99-305:15454] Signal: Aborted (6)
[fv-az99-305:15454] Signal code:  (-6)
[fv-az99-305:15454] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f5ae0f5e210]
[fv-az99-305:15454] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f5ae0f5e18b]
[fv-az99-305:15454] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f5ae0f3d859]
[fv-az99-305:15454] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f5ae11c5951]
[fv-az99-305:15454] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f5ae11d147c]
[fv-az99-305:15454] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f5ae11d14e7]
[fv-az99-305:15454] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f5ae11d1799]
[fv-az99-305:15454] [ 7] plumed(+0xf47d)[0x55ecee8cc47d]
[fv-az99-305:15454] [ 8] plumed(+0x14004)[0x55ecee8d1004]
[fv-az99-305:15454] [ 9] plumed(+0xf698)[0x55ecee8cc698]
[fv-az99-305:15454] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f5ae0f3f0b3]
[fv-az99-305:15454] [11] plumed(+0xf76e)[0x55ecee8cc76e]
[fv-az99-305:15454] *** End of error message ***
</pre>
{% endraw %}
