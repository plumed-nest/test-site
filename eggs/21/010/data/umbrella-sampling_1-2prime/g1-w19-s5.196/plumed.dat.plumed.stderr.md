**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w19-s5.196/plumed.dat   
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
[fv-az99-305:08787] *** Process received signal ***
[fv-az99-305:08787] Signal: Aborted (6)
[fv-az99-305:08787] Signal code:  (-6)
[fv-az99-305:08787] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f7e15bee210]
[fv-az99-305:08787] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f7e15bee18b]
[fv-az99-305:08787] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f7e15bcd859]
[fv-az99-305:08787] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f7e15e55951]
[fv-az99-305:08787] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f7e15e6147c]
[fv-az99-305:08787] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f7e15e614e7]
[fv-az99-305:08787] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f7e15e61799]
[fv-az99-305:08787] [ 7] plumed(+0xf47d)[0x5578de11347d]
[fv-az99-305:08787] [ 8] plumed(+0x14004)[0x5578de118004]
[fv-az99-305:08787] [ 9] plumed(+0xf698)[0x5578de113698]
[fv-az99-305:08787] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f7e15bcf0b3]
[fv-az99-305:08787] [11] plumed(+0xf76e)[0x5578de11376e]
[fv-az99-305:08787] *** End of error message ***
</pre>
{% endraw %}
