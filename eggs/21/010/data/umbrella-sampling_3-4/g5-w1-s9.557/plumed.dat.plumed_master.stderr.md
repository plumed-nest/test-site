**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_3-4/g5-w1-s9.557/plumed.dat   
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
[fv-az99-305:12642] *** Process received signal ***
[fv-az99-305:12642] Signal: Aborted (6)
[fv-az99-305:12642] Signal code:  (-6)
[fv-az99-305:12642] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fa0a6784210]
[fv-az99-305:12642] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fa0a678418b]
[fv-az99-305:12642] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fa0a6763859]
[fv-az99-305:12642] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fa0a69eb951]
[fv-az99-305:12642] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fa0a69f747c]
[fv-az99-305:12642] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fa0a69f74e7]
[fv-az99-305:12642] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7fa0a69f77ed]
[fv-az99-305:12642] [ 7] plumed_master(+0xf568)[0x558137753568]
[fv-az99-305:12642] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fa0a67650b3]
[fv-az99-305:12642] [ 9] plumed_master(+0xf79e)[0x55813775379e]
[fv-az99-305:12642] *** End of error message ***
</pre>
{% endraw %}
