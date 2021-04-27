**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w29-s7.356/plumed.dat   
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
[fv-az99-305:09058] *** Process received signal ***
[fv-az99-305:09058] Signal: Aborted (6)
[fv-az99-305:09058] Signal code:  (-6)
[fv-az99-305:09058] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fd08f3c3210]
[fv-az99-305:09058] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fd08f3c318b]
[fv-az99-305:09058] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fd08f3a2859]
[fv-az99-305:09058] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fd08f62a951]
[fv-az99-305:09058] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fd08f63647c]
[fv-az99-305:09058] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fd08f6364e7]
[fv-az99-305:09058] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fd08f636799]
[fv-az99-305:09058] [ 7] plumed(+0xf47d)[0x558e2b10547d]
[fv-az99-305:09058] [ 8] plumed(+0x14004)[0x558e2b10a004]
[fv-az99-305:09058] [ 9] plumed(+0xf698)[0x558e2b105698]
[fv-az99-305:09058] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fd08f3a40b3]
[fv-az99-305:09058] [11] plumed(+0xf76e)[0x558e2b10576e]
[fv-az99-305:09058] *** End of error message ***
</pre>
{% endraw %}
