**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_4-5prime/g3-w1-s3.1135/plumed.dat   
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
[fv-az99-305:14328] *** Process received signal ***
[fv-az99-305:14328] Signal: Aborted (6)
[fv-az99-305:14328] Signal code:  (-6)
[fv-az99-305:14328] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fb7c6673210]
[fv-az99-305:14328] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fb7c667318b]
[fv-az99-305:14328] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fb7c6652859]
[fv-az99-305:14328] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fb7c68da951]
[fv-az99-305:14328] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fb7c68e647c]
[fv-az99-305:14328] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fb7c68e64e7]
[fv-az99-305:14328] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fb7c68e6799]
[fv-az99-305:14328] [ 7] plumed(+0xf47d)[0x56254ab3c47d]
[fv-az99-305:14328] [ 8] plumed(+0x14004)[0x56254ab41004]
[fv-az99-305:14328] [ 9] plumed(+0xf698)[0x56254ab3c698]
[fv-az99-305:14328] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fb7c66540b3]
[fv-az99-305:14328] [11] plumed(+0xf76e)[0x56254ab3c76e]
[fv-az99-305:14328] *** End of error message ***
</pre>
{% endraw %}
