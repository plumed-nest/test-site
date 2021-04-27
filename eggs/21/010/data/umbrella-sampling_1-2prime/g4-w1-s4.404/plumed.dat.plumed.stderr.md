**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g4-w1-s4.404/plumed.dat   
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
[fv-az99-305:09844] *** Process received signal ***
[fv-az99-305:09844] Signal: Aborted (6)
[fv-az99-305:09844] Signal code:  (-6)
[fv-az99-305:09844] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fc3ef434210]
[fv-az99-305:09844] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fc3ef43418b]
[fv-az99-305:09844] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fc3ef413859]
[fv-az99-305:09844] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fc3ef69b951]
[fv-az99-305:09844] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fc3ef6a747c]
[fv-az99-305:09844] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fc3ef6a74e7]
[fv-az99-305:09844] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fc3ef6a7799]
[fv-az99-305:09844] [ 7] plumed(+0xf47d)[0x56469c1b247d]
[fv-az99-305:09844] [ 8] plumed(+0x14004)[0x56469c1b7004]
[fv-az99-305:09844] [ 9] plumed(+0xf698)[0x56469c1b2698]
[fv-az99-305:09844] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fc3ef4150b3]
[fv-az99-305:09844] [11] plumed(+0xf76e)[0x56469c1b276e]
[fv-az99-305:09844] *** End of error message ***
</pre>
{% endraw %}
