**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_2-3/g1-w6-s6.308/plumed.dat   
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
[fv-az99-305:10539] *** Process received signal ***
[fv-az99-305:10539] Signal: Aborted (6)
[fv-az99-305:10539] Signal code:  (-6)
[fv-az99-305:10539] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f686f9f6210]
[fv-az99-305:10539] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f686f9f618b]
[fv-az99-305:10539] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f686f9d5859]
[fv-az99-305:10539] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f686fc5d951]
[fv-az99-305:10539] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f686fc6947c]
[fv-az99-305:10539] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f686fc694e7]
[fv-az99-305:10539] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7f686fc697ed]
[fv-az99-305:10539] [ 7] plumed_master(+0xf568)[0x55b7e8896568]
[fv-az99-305:10539] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f686f9d70b3]
[fv-az99-305:10539] [ 9] plumed_master(+0xf79e)[0x55b7e889679e]
[fv-az99-305:10539] *** End of error message ***
</pre>
{% endraw %}
