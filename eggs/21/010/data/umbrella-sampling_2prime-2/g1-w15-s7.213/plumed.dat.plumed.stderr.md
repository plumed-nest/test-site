**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_2prime-2/g1-w15-s7.213/plumed.dat   
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
[fv-az99-305:10966] *** Process received signal ***
[fv-az99-305:10966] Signal: Aborted (6)
[fv-az99-305:10966] Signal code:  (-6)
[fv-az99-305:10966] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fd493a84210]
[fv-az99-305:10966] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fd493a8418b]
[fv-az99-305:10966] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fd493a63859]
[fv-az99-305:10966] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fd493ceb951]
[fv-az99-305:10966] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fd493cf747c]
[fv-az99-305:10966] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fd493cf74e7]
[fv-az99-305:10966] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fd493cf7799]
[fv-az99-305:10966] [ 7] plumed(+0xf47d)[0x55ba3b63847d]
[fv-az99-305:10966] [ 8] plumed(+0x14004)[0x55ba3b63d004]
[fv-az99-305:10966] [ 9] plumed(+0xf698)[0x55ba3b638698]
[fv-az99-305:10966] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fd493a650b3]
[fv-az99-305:10966] [11] plumed(+0xf76e)[0x55ba3b63876e]
[fv-az99-305:10966] *** End of error message ***
</pre>
{% endraw %}
