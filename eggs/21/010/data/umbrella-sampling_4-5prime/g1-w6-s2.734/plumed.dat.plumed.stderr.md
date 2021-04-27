**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_4-5prime/g1-w6-s2.734/plumed.dat   
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
[fv-az99-305:14131] *** Process received signal ***
[fv-az99-305:14131] Signal: Aborted (6)
[fv-az99-305:14131] Signal code:  (-6)
[fv-az99-305:14131] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f68f5f2e210]
[fv-az99-305:14131] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f68f5f2e18b]
[fv-az99-305:14131] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f68f5f0d859]
[fv-az99-305:14131] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f68f6195951]
[fv-az99-305:14131] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f68f61a147c]
[fv-az99-305:14131] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f68f61a14e7]
[fv-az99-305:14131] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f68f61a1799]
[fv-az99-305:14131] [ 7] plumed(+0xf47d)[0x55dba446547d]
[fv-az99-305:14131] [ 8] plumed(+0x14004)[0x55dba446a004]
[fv-az99-305:14131] [ 9] plumed(+0xf698)[0x55dba4465698]
[fv-az99-305:14131] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f68f5f0f0b3]
[fv-az99-305:14131] [11] plumed(+0xf76e)[0x55dba446576e]
[fv-az99-305:14131] *** End of error message ***
</pre>
{% endraw %}
