**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w14-s4.116/plumed.dat   
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
[fv-az99-305:08662] *** Process received signal ***
[fv-az99-305:08662] Signal: Aborted (6)
[fv-az99-305:08662] Signal code:  (-6)
[fv-az99-305:08662] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7ff880193210]
[fv-az99-305:08662] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7ff88019318b]
[fv-az99-305:08662] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7ff880172859]
[fv-az99-305:08662] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7ff8803fa951]
[fv-az99-305:08662] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7ff88040647c]
[fv-az99-305:08662] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7ff8804064e7]
[fv-az99-305:08662] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7ff880406799]
[fv-az99-305:08662] [ 7] plumed(+0xf47d)[0x558ae598747d]
[fv-az99-305:08662] [ 8] plumed(+0x14004)[0x558ae598c004]
[fv-az99-305:08662] [ 9] plumed(+0xf698)[0x558ae5987698]
[fv-az99-305:08662] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7ff8801740b3]
[fv-az99-305:08662] [11] plumed(+0xf76e)[0x558ae598776e]
[fv-az99-305:08662] *** End of error message ***
</pre>
{% endraw %}
