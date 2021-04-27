**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_2prime-2/g3-w1-s2.249/plumed.dat   
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
[fv-az99-305:11504] *** Process received signal ***
[fv-az99-305:11504] Signal: Aborted (6)
[fv-az99-305:11504] Signal code:  (-6)
[fv-az99-305:11504] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fbf69aaa210]
[fv-az99-305:11504] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fbf69aaa18b]
[fv-az99-305:11504] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fbf69a89859]
[fv-az99-305:11504] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fbf69d11951]
[fv-az99-305:11504] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fbf69d1d47c]
[fv-az99-305:11504] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fbf69d1d4e7]
[fv-az99-305:11504] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fbf69d1d799]
[fv-az99-305:11504] [ 7] plumed(+0xf47d)[0x557a4251647d]
[fv-az99-305:11504] [ 8] plumed(+0x14004)[0x557a4251b004]
[fv-az99-305:11504] [ 9] plumed(+0xf698)[0x557a42516698]
[fv-az99-305:11504] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fbf69a8b0b3]
[fv-az99-305:11504] [11] plumed(+0xf76e)[0x557a4251676e]
[fv-az99-305:11504] *** End of error message ***
</pre>
{% endraw %}
