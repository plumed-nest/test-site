**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_5prime-5/g1-w3-s2.750/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:704, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: HILLS RESTART HEIGHT 0.000 W_STRIDE 50
Maybe a missing space or a typo?
[fv-az99-305:16151] *** Process received signal ***
[fv-az99-305:16151] Signal: Aborted (6)
[fv-az99-305:16151] Signal code:  (-6)
[fv-az99-305:16151] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f7a087da210]
[fv-az99-305:16151] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f7a087da18b]
[fv-az99-305:16151] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f7a087b9859]
[fv-az99-305:16151] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f7a08a41951]
[fv-az99-305:16151] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f7a08a4d47c]
[fv-az99-305:16151] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f7a08a4d4e7]
[fv-az99-305:16151] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7f7a08a4d7ed]
[fv-az99-305:16151] [ 7] plumed_master(+0xf568)[0x55820c665568]
[fv-az99-305:16151] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f7a087bb0b3]
[fv-az99-305:16151] [ 9] plumed_master(+0xf79e)[0x55820c66579e]
[fv-az99-305:16151] *** End of error message ***
</pre>
{% endraw %}
