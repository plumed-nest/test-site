**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_4-5prime/g2-w2-s5.8435/plumed.dat   
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
[fv-az99-305:14279] *** Process received signal ***
[fv-az99-305:14279] Signal: Aborted (6)
[fv-az99-305:14279] Signal code:  (-6)
[fv-az99-305:14279] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fef4c4f3210]
[fv-az99-305:14279] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fef4c4f318b]
[fv-az99-305:14279] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fef4c4d2859]
[fv-az99-305:14279] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fef4c75a951]
[fv-az99-305:14279] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fef4c76647c]
[fv-az99-305:14279] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fef4c7664e7]
[fv-az99-305:14279] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fef4c766799]
[fv-az99-305:14279] [ 7] plumed(+0xf47d)[0x5571c9ee847d]
[fv-az99-305:14279] [ 8] plumed(+0x14004)[0x5571c9eed004]
[fv-az99-305:14279] [ 9] plumed(+0xf698)[0x5571c9ee8698]
[fv-az99-305:14279] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fef4c4d40b3]
[fv-az99-305:14279] [11] plumed(+0xf76e)[0x5571c9ee876e]
[fv-az99-305:14279] *** End of error message ***
</pre>
{% endraw %}
