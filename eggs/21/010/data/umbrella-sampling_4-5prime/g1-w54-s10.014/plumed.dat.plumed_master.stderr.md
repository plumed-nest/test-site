**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_4-5prime/g1-w54-s10.014/plumed.dat   
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
[fv-az99-305:13993] *** Process received signal ***
[fv-az99-305:13993] Signal: Aborted (6)
[fv-az99-305:13993] Signal code:  (-6)
[fv-az99-305:13993] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fd30f848210]
[fv-az99-305:13993] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fd30f84818b]
[fv-az99-305:13993] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fd30f827859]
[fv-az99-305:13993] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fd30faaf951]
[fv-az99-305:13993] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fd30fabb47c]
[fv-az99-305:13993] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fd30fabb4e7]
[fv-az99-305:13993] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7fd30fabb7ed]
[fv-az99-305:13993] [ 7] plumed_master(+0xf568)[0x55be9954f568]
[fv-az99-305:13993] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fd30f8290b3]
[fv-az99-305:13993] [ 9] plumed_master(+0xf79e)[0x55be9954f79e]
[fv-az99-305:13993] *** End of error message ***
</pre>
{% endraw %}
