**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_5-6/g1-w6-s2.875/plumed.dat   
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
[fv-az99-305:15257] *** Process received signal ***
[fv-az99-305:15257] Signal: Aborted (6)
[fv-az99-305:15257] Signal code:  (-6)
[fv-az99-305:15257] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f897e357210]
[fv-az99-305:15257] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f897e35718b]
[fv-az99-305:15257] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f897e336859]
[fv-az99-305:15257] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f897e5be951]
[fv-az99-305:15257] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f897e5ca47c]
[fv-az99-305:15257] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f897e5ca4e7]
[fv-az99-305:15257] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f897e5ca799]
[fv-az99-305:15257] [ 7] plumed(+0xf47d)[0x56483af9847d]
[fv-az99-305:15257] [ 8] plumed(+0x14004)[0x56483af9d004]
[fv-az99-305:15257] [ 9] plumed(+0xf698)[0x56483af98698]
[fv-az99-305:15257] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f897e3380b3]
[fv-az99-305:15257] [11] plumed(+0xf76e)[0x56483af9876e]
[fv-az99-305:15257] *** End of error message ***
</pre>
{% endraw %}
