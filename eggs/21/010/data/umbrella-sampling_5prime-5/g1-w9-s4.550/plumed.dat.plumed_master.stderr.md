**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_5prime-5/g1-w9-s4.550/plumed.dat   
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
[fv-az99-305:16323] *** Process received signal ***
[fv-az99-305:16323] Signal: Aborted (6)
[fv-az99-305:16323] Signal code:  (-6)
[fv-az99-305:16323] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fe2b5e63210]
[fv-az99-305:16323] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fe2b5e6318b]
[fv-az99-305:16323] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fe2b5e42859]
[fv-az99-305:16323] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fe2b60ca951]
[fv-az99-305:16323] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fe2b60d647c]
[fv-az99-305:16323] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fe2b60d64e7]
[fv-az99-305:16323] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7fe2b60d67ed]
[fv-az99-305:16323] [ 7] plumed_master(+0xf568)[0x55fdfbe40568]
[fv-az99-305:16323] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fe2b5e440b3]
[fv-az99-305:16323] [ 9] plumed_master(+0xf79e)[0x55fdfbe4079e]
[fv-az99-305:16323] *** End of error message ***
</pre>
{% endraw %}
