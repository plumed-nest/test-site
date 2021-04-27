**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_2-3/g1-w22-s9.242/plumed.dat   
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
[fv-az99-305:10334] *** Process received signal ***
[fv-az99-305:10334] Signal: Aborted (6)
[fv-az99-305:10334] Signal code:  (-6)
[fv-az99-305:10334] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fa6f708c210]
[fv-az99-305:10334] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fa6f708c18b]
[fv-az99-305:10334] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fa6f706b859]
[fv-az99-305:10334] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fa6f72f3951]
[fv-az99-305:10334] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fa6f72ff47c]
[fv-az99-305:10334] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fa6f72ff4e7]
[fv-az99-305:10334] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fa6f72ff799]
[fv-az99-305:10334] [ 7] plumed(+0xf47d)[0x55e71c17f47d]
[fv-az99-305:10334] [ 8] plumed(+0x14004)[0x55e71c184004]
[fv-az99-305:10334] [ 9] plumed(+0xf698)[0x55e71c17f698]
[fv-az99-305:10334] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fa6f706d0b3]
[fv-az99-305:10334] [11] plumed(+0xf76e)[0x55e71c17f76e]
[fv-az99-305:10334] *** End of error message ***
</pre>
{% endraw %}
