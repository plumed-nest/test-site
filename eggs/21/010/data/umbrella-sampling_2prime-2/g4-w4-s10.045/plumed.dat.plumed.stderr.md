**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_2prime-2/g4-w4-s10.045/plumed.dat   
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
[fv-az99-305:11726] *** Process received signal ***
[fv-az99-305:11726] Signal: Aborted (6)
[fv-az99-305:11726] Signal code:  (-6)
[fv-az99-305:11726] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fc0076f4210]
[fv-az99-305:11726] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fc0076f418b]
[fv-az99-305:11726] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fc0076d3859]
[fv-az99-305:11726] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fc00795b951]
[fv-az99-305:11726] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fc00796747c]
[fv-az99-305:11726] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fc0079674e7]
[fv-az99-305:11726] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fc007967799]
[fv-az99-305:11726] [ 7] plumed(+0xf47d)[0x55b98206647d]
[fv-az99-305:11726] [ 8] plumed(+0x14004)[0x55b98206b004]
[fv-az99-305:11726] [ 9] plumed(+0xf698)[0x55b982066698]
[fv-az99-305:11726] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fc0076d50b3]
[fv-az99-305:11726] [11] plumed(+0xf76e)[0x55b98206676e]
[fv-az99-305:11726] *** End of error message ***
</pre>
{% endraw %}
