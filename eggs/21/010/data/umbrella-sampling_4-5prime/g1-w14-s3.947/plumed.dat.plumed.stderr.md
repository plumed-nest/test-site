**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_4-5prime/g1-w14-s3.947/plumed.dat   
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
[fv-az99-305:12908] *** Process received signal ***
[fv-az99-305:12908] Signal: Aborted (6)
[fv-az99-305:12908] Signal code:  (-6)
[fv-az99-305:12908] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7eff94bf3210]
[fv-az99-305:12908] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7eff94bf318b]
[fv-az99-305:12908] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7eff94bd2859]
[fv-az99-305:12908] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7eff94e5a951]
[fv-az99-305:12908] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7eff94e6647c]
[fv-az99-305:12908] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7eff94e664e7]
[fv-az99-305:12908] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7eff94e66799]
[fv-az99-305:12908] [ 7] plumed(+0xf47d)[0x5558ea9ff47d]
[fv-az99-305:12908] [ 8] plumed(+0x14004)[0x5558eaa04004]
[fv-az99-305:12908] [ 9] plumed(+0xf698)[0x5558ea9ff698]
[fv-az99-305:12908] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7eff94bd40b3]
[fv-az99-305:12908] [11] plumed(+0xf76e)[0x5558ea9ff76e]
[fv-az99-305:12908] *** End of error message ***
</pre>
{% endraw %}
