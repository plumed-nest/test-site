**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_4-5prime/g1-w41-s8.043/plumed.dat   
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
[fv-az99-305:13644] *** Process received signal ***
[fv-az99-305:13644] Signal: Aborted (6)
[fv-az99-305:13644] Signal code:  (-6)
[fv-az99-305:13644] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7ff44e107210]
[fv-az99-305:13644] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7ff44e10718b]
[fv-az99-305:13644] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7ff44e0e6859]
[fv-az99-305:13644] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7ff44e36e951]
[fv-az99-305:13644] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7ff44e37a47c]
[fv-az99-305:13644] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7ff44e37a4e7]
[fv-az99-305:13644] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7ff44e37a799]
[fv-az99-305:13644] [ 7] plumed(+0xf47d)[0x5575d7d9747d]
[fv-az99-305:13644] [ 8] plumed(+0x14004)[0x5575d7d9c004]
[fv-az99-305:13644] [ 9] plumed(+0xf698)[0x5575d7d97698]
[fv-az99-305:13644] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7ff44e0e80b3]
[fv-az99-305:13644] [11] plumed(+0xf76e)[0x5575d7d9776e]
[fv-az99-305:13644] *** End of error message ***
</pre>
{% endraw %}
