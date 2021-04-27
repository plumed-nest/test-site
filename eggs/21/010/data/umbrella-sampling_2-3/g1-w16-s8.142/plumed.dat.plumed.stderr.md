**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_2-3/g1-w16-s8.142/plumed.dat   
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
[fv-az99-305:10115] *** Process received signal ***
[fv-az99-305:10115] Signal: Aborted (6)
[fv-az99-305:10115] Signal code:  (-6)
[fv-az99-305:10115] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fc176a60210]
[fv-az99-305:10115] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fc176a6018b]
[fv-az99-305:10115] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fc176a3f859]
[fv-az99-305:10115] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fc176cc7951]
[fv-az99-305:10115] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fc176cd347c]
[fv-az99-305:10115] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fc176cd34e7]
[fv-az99-305:10115] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fc176cd3799]
[fv-az99-305:10115] [ 7] plumed(+0xf47d)[0x558e0fd0747d]
[fv-az99-305:10115] [ 8] plumed(+0x14004)[0x558e0fd0c004]
[fv-az99-305:10115] [ 9] plumed(+0xf698)[0x558e0fd07698]
[fv-az99-305:10115] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fc176a410b3]
[fv-az99-305:10115] [11] plumed(+0xf76e)[0x558e0fd0776e]
[fv-az99-305:10115] *** End of error message ***
</pre>
{% endraw %}
