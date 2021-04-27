**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_5-6/g1-w15-s5.125/plumed.dat   
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
[fv-az99-305:14525] *** Process received signal ***
[fv-az99-305:14525] Signal: Aborted (6)
[fv-az99-305:14525] Signal code:  (-6)
[fv-az99-305:14525] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fd0a3edf210]
[fv-az99-305:14525] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fd0a3edf18b]
[fv-az99-305:14525] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fd0a3ebe859]
[fv-az99-305:14525] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fd0a4146951]
[fv-az99-305:14525] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fd0a415247c]
[fv-az99-305:14525] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fd0a41524e7]
[fv-az99-305:14525] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fd0a4152799]
[fv-az99-305:14525] [ 7] plumed(+0xf47d)[0x5653e524347d]
[fv-az99-305:14525] [ 8] plumed(+0x14004)[0x5653e5248004]
[fv-az99-305:14525] [ 9] plumed(+0xf698)[0x5653e5243698]
[fv-az99-305:14525] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fd0a3ec00b3]
[fv-az99-305:14525] [11] plumed(+0xf76e)[0x5653e524376e]
[fv-az99-305:14525] *** End of error message ***
</pre>
{% endraw %}
