**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_4-5prime/g1-w10-s3.341/plumed.dat   
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
[fv-az99-305:12807] *** Process received signal ***
[fv-az99-305:12807] Signal: Aborted (6)
[fv-az99-305:12807] Signal code:  (-6)
[fv-az99-305:12807] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fbd84750210]
[fv-az99-305:12807] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fbd8475018b]
[fv-az99-305:12807] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fbd8472f859]
[fv-az99-305:12807] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fbd849b7951]
[fv-az99-305:12807] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fbd849c347c]
[fv-az99-305:12807] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fbd849c34e7]
[fv-az99-305:12807] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fbd849c3799]
[fv-az99-305:12807] [ 7] plumed(+0xf47d)[0x563250c7d47d]
[fv-az99-305:12807] [ 8] plumed(+0x14004)[0x563250c82004]
[fv-az99-305:12807] [ 9] plumed(+0xf698)[0x563250c7d698]
[fv-az99-305:12807] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fbd847310b3]
[fv-az99-305:12807] [11] plumed(+0xf76e)[0x563250c7d76e]
[fv-az99-305:12807] *** End of error message ***
</pre>
{% endraw %}
