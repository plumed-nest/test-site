**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w38-s9.300/plumed.dat   
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
[fv-az99-305:09302] *** Process received signal ***
[fv-az99-305:09302] Signal: Aborted (6)
[fv-az99-305:09302] Signal code:  (-6)
[fv-az99-305:09302] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f6e42fc7210]
[fv-az99-305:09302] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f6e42fc718b]
[fv-az99-305:09302] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f6e42fa6859]
[fv-az99-305:09302] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f6e4322e951]
[fv-az99-305:09302] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f6e4323a47c]
[fv-az99-305:09302] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f6e4323a4e7]
[fv-az99-305:09302] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f6e4323a799]
[fv-az99-305:09302] [ 7] plumed(+0xf47d)[0x559eb564a47d]
[fv-az99-305:09302] [ 8] plumed(+0x14004)[0x559eb564f004]
[fv-az99-305:09302] [ 9] plumed(+0xf698)[0x559eb564a698]
[fv-az99-305:09302] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f6e42fa80b3]
[fv-az99-305:09302] [11] plumed(+0xf76e)[0x559eb564a76e]
[fv-az99-305:09302] *** End of error message ***
</pre>
{% endraw %}
