**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_2-3/g1-w10-s7.042/plumed.dat   
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
[fv-az99-305:09969] *** Process received signal ***
[fv-az99-305:09969] Signal: Aborted (6)
[fv-az99-305:09969] Signal code:  (-6)
[fv-az99-305:09969] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f6615af3210]
[fv-az99-305:09969] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f6615af318b]
[fv-az99-305:09969] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f6615ad2859]
[fv-az99-305:09969] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f6615d5a951]
[fv-az99-305:09969] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f6615d6647c]
[fv-az99-305:09969] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f6615d664e7]
[fv-az99-305:09969] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f6615d66799]
[fv-az99-305:09969] [ 7] plumed(+0xf47d)[0x559a458d347d]
[fv-az99-305:09969] [ 8] plumed(+0x14004)[0x559a458d8004]
[fv-az99-305:09969] [ 9] plumed(+0xf698)[0x559a458d3698]
[fv-az99-305:09969] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f6615ad40b3]
[fv-az99-305:09969] [11] plumed(+0xf76e)[0x559a458d376e]
[fv-az99-305:09969] *** End of error message ***
</pre>
{% endraw %}
