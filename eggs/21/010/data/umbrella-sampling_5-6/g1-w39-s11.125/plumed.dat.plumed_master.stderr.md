**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_5-6/g1-w39-s11.125/plumed.dat   
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
[fv-az99-305:15168] *** Process received signal ***
[fv-az99-305:15168] Signal: Aborted (6)
[fv-az99-305:15168] Signal code:  (-6)
[fv-az99-305:15168] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fa5979b5210]
[fv-az99-305:15168] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fa5979b518b]
[fv-az99-305:15168] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fa597994859]
[fv-az99-305:15168] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fa597c1c951]
[fv-az99-305:15168] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fa597c2847c]
[fv-az99-305:15168] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fa597c284e7]
[fv-az99-305:15168] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7fa597c287ed]
[fv-az99-305:15168] [ 7] plumed_master(+0xf568)[0x557a638e4568]
[fv-az99-305:15168] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fa5979960b3]
[fv-az99-305:15168] [ 9] plumed_master(+0xf79e)[0x557a638e479e]
[fv-az99-305:15168] *** End of error message ***
</pre>
{% endraw %}
