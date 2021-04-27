**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_4-5prime/g1-w58-s10.621/plumed.dat   
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
[fv-az99-305:14090] *** Process received signal ***
[fv-az99-305:14090] Signal: Aborted (6)
[fv-az99-305:14090] Signal code:  (-6)
[fv-az99-305:14090] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f6d4ebc7210]
[fv-az99-305:14090] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f6d4ebc718b]
[fv-az99-305:14090] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f6d4eba6859]
[fv-az99-305:14090] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f6d4ee2e951]
[fv-az99-305:14090] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f6d4ee3a47c]
[fv-az99-305:14090] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f6d4ee3a4e7]
[fv-az99-305:14090] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7f6d4ee3a7ed]
[fv-az99-305:14090] [ 7] plumed_master(+0xf568)[0x562dd528c568]
[fv-az99-305:14090] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f6d4eba80b3]
[fv-az99-305:14090] [ 9] plumed_master(+0xf79e)[0x562dd528c79e]
[fv-az99-305:14090] *** End of error message ***
</pre>
{% endraw %}
