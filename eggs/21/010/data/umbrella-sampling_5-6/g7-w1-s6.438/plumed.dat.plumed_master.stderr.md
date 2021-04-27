**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_5-6/g7-w1-s6.438/plumed.dat   
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
[fv-az99-305:15560] *** Process received signal ***
[fv-az99-305:15560] Signal: Aborted (6)
[fv-az99-305:15560] Signal code:  (-6)
[fv-az99-305:15560] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f83c2e10210]
[fv-az99-305:15560] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f83c2e1018b]
[fv-az99-305:15560] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f83c2def859]
[fv-az99-305:15560] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f83c3077951]
[fv-az99-305:15560] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f83c308347c]
[fv-az99-305:15560] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f83c30834e7]
[fv-az99-305:15560] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7f83c30837ed]
[fv-az99-305:15560] [ 7] plumed_master(+0xf568)[0x560e182d8568]
[fv-az99-305:15560] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f83c2df10b3]
[fv-az99-305:15560] [ 9] plumed_master(+0xf79e)[0x560e182d879e]
[fv-az99-305:15560] *** End of error message ***
</pre>
{% endraw %}
