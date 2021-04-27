**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_4-5prime/g1-w28-s6.071/plumed.dat   
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
[fv-az99-305:13276] *** Process received signal ***
[fv-az99-305:13276] Signal: Aborted (6)
[fv-az99-305:13276] Signal code:  (-6)
[fv-az99-305:13276] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fa718d32210]
[fv-az99-305:13276] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fa718d3218b]
[fv-az99-305:13276] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fa718d11859]
[fv-az99-305:13276] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fa718f99951]
[fv-az99-305:13276] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fa718fa547c]
[fv-az99-305:13276] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fa718fa54e7]
[fv-az99-305:13276] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fa718fa5799]
[fv-az99-305:13276] [ 7] plumed(+0xf47d)[0x5633d76ba47d]
[fv-az99-305:13276] [ 8] plumed(+0x14004)[0x5633d76bf004]
[fv-az99-305:13276] [ 9] plumed(+0xf698)[0x5633d76ba698]
[fv-az99-305:13276] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fa718d130b3]
[fv-az99-305:13276] [11] plumed(+0xf76e)[0x5633d76ba76e]
[fv-az99-305:13276] *** End of error message ***
</pre>
{% endraw %}
