**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_4-5prime/g1-w22-s5.161/plumed.dat   
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
[fv-az99-305:13129] *** Process received signal ***
[fv-az99-305:13129] Signal: Aborted (6)
[fv-az99-305:13129] Signal code:  (-6)
[fv-az99-305:13129] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f2a5cd61210]
[fv-az99-305:13129] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f2a5cd6118b]
[fv-az99-305:13129] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f2a5cd40859]
[fv-az99-305:13129] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f2a5cfc8951]
[fv-az99-305:13129] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f2a5cfd447c]
[fv-az99-305:13129] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f2a5cfd44e7]
[fv-az99-305:13129] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f2a5cfd4799]
[fv-az99-305:13129] [ 7] plumed(+0xf47d)[0x55949fc3f47d]
[fv-az99-305:13129] [ 8] plumed(+0x14004)[0x55949fc44004]
[fv-az99-305:13129] [ 9] plumed(+0xf698)[0x55949fc3f698]
[fv-az99-305:13129] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f2a5cd420b3]
[fv-az99-305:13129] [11] plumed(+0xf76e)[0x55949fc3f76e]
[fv-az99-305:13129] *** End of error message ***
</pre>
{% endraw %}
