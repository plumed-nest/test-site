**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_3-4/g2-w9-s4.957/plumed.dat   
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
[fv-az99-305:12461] *** Process received signal ***
[fv-az99-305:12461] Signal: Aborted (6)
[fv-az99-305:12461] Signal code:  (-6)
[fv-az99-305:12461] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fc1b09f4210]
[fv-az99-305:12461] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fc1b09f418b]
[fv-az99-305:12461] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fc1b09d3859]
[fv-az99-305:12461] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fc1b0c5b951]
[fv-az99-305:12461] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fc1b0c6747c]
[fv-az99-305:12461] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fc1b0c674e7]
[fv-az99-305:12461] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fc1b0c67799]
[fv-az99-305:12461] [ 7] plumed(+0xf47d)[0x55fa87e4b47d]
[fv-az99-305:12461] [ 8] plumed(+0x14004)[0x55fa87e50004]
[fv-az99-305:12461] [ 9] plumed(+0xf698)[0x55fa87e4b698]
[fv-az99-305:12461] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fc1b09d50b3]
[fv-az99-305:12461] [11] plumed(+0xf76e)[0x55fa87e4b76e]
[fv-az99-305:12461] *** End of error message ***
</pre>
{% endraw %}
