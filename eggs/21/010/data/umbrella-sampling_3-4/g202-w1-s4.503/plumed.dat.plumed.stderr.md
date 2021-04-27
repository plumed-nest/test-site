**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_3-4/g202-w1-s4.503/plumed.dat   
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
[fv-az99-305:12535] *** Process received signal ***
[fv-az99-305:12535] Signal: Aborted (6)
[fv-az99-305:12535] Signal code:  (-6)
[fv-az99-305:12535] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f9d5ca3f210]
[fv-az99-305:12535] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f9d5ca3f18b]
[fv-az99-305:12535] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f9d5ca1e859]
[fv-az99-305:12535] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f9d5cca6951]
[fv-az99-305:12535] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f9d5ccb247c]
[fv-az99-305:12535] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f9d5ccb24e7]
[fv-az99-305:12535] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f9d5ccb2799]
[fv-az99-305:12535] [ 7] plumed(+0xf47d)[0x56036e6bb47d]
[fv-az99-305:12535] [ 8] plumed(+0x14004)[0x56036e6c0004]
[fv-az99-305:12535] [ 9] plumed(+0xf698)[0x56036e6bb698]
[fv-az99-305:12535] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f9d5ca200b3]
[fv-az99-305:12535] [11] plumed(+0xf76e)[0x56036e6bb76e]
[fv-az99-305:12535] *** End of error message ***
</pre>
{% endraw %}
