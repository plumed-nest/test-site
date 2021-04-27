**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_5-6/g1-w6-s2.875/plumed.dat   
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
[fv-az99-305:15265] *** Process received signal ***
[fv-az99-305:15265] Signal: Aborted (6)
[fv-az99-305:15265] Signal code:  (-6)
[fv-az99-305:15265] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f2d6651f210]
[fv-az99-305:15265] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f2d6651f18b]
[fv-az99-305:15265] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f2d664fe859]
[fv-az99-305:15265] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f2d66786951]
[fv-az99-305:15265] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f2d6679247c]
[fv-az99-305:15265] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f2d667924e7]
[fv-az99-305:15265] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7f2d667927ed]
[fv-az99-305:15265] [ 7] plumed_master(+0xf568)[0x5587f1388568]
[fv-az99-305:15265] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f2d665000b3]
[fv-az99-305:15265] [ 9] plumed_master(+0xf79e)[0x5587f138879e]
[fv-az99-305:15265] *** End of error message ***
</pre>
{% endraw %}
