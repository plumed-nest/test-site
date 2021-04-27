**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_4-5prime/g1-w34-s6.981/plumed.dat   
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
[fv-az99-305:13456] *** Process received signal ***
[fv-az99-305:13456] Signal: Aborted (6)
[fv-az99-305:13456] Signal code:  (-6)
[fv-az99-305:13456] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7ff542844210]
[fv-az99-305:13456] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7ff54284418b]
[fv-az99-305:13456] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7ff542823859]
[fv-az99-305:13456] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7ff542aab951]
[fv-az99-305:13456] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7ff542ab747c]
[fv-az99-305:13456] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7ff542ab74e7]
[fv-az99-305:13456] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7ff542ab77ed]
[fv-az99-305:13456] [ 7] plumed_master(+0xf568)[0x564d3fe87568]
[fv-az99-305:13456] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7ff5428250b3]
[fv-az99-305:13456] [ 9] plumed_master(+0xf79e)[0x564d3fe8779e]
[fv-az99-305:13456] *** End of error message ***
</pre>
{% endraw %}
