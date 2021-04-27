**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_5prime-5/g1-w24-s9.050/plumed.dat   
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
[fv-az99-305:15998] *** Process received signal ***
[fv-az99-305:15998] Signal: Aborted (6)
[fv-az99-305:15998] Signal code:  (-6)
[fv-az99-305:15998] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f17ee777210]
[fv-az99-305:15998] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f17ee77718b]
[fv-az99-305:15998] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f17ee756859]
[fv-az99-305:15998] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f17ee9de951]
[fv-az99-305:15998] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f17ee9ea47c]
[fv-az99-305:15998] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f17ee9ea4e7]
[fv-az99-305:15998] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f17ee9ea799]
[fv-az99-305:15998] [ 7] plumed(+0xf47d)[0x55cddd3d547d]
[fv-az99-305:15998] [ 8] plumed(+0x14004)[0x55cddd3da004]
[fv-az99-305:15998] [ 9] plumed(+0xf698)[0x55cddd3d5698]
[fv-az99-305:15998] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f17ee7580b3]
[fv-az99-305:15998] [11] plumed(+0xf76e)[0x55cddd3d576e]
[fv-az99-305:15998] *** End of error message ***
</pre>
{% endraw %}
