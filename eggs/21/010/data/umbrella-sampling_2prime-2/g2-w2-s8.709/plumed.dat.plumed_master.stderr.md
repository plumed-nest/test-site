**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_2prime-2/g2-w2-s8.709/plumed.dat   
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
[fv-az99-305:11488] *** Process received signal ***
[fv-az99-305:11488] Signal: Aborted (6)
[fv-az99-305:11488] Signal code:  (-6)
[fv-az99-305:11488] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7ff2b3448210]
[fv-az99-305:11488] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7ff2b344818b]
[fv-az99-305:11488] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7ff2b3427859]
[fv-az99-305:11488] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7ff2b36af951]
[fv-az99-305:11488] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7ff2b36bb47c]
[fv-az99-305:11488] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7ff2b36bb4e7]
[fv-az99-305:11488] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7ff2b36bb7ed]
[fv-az99-305:11488] [ 7] plumed_master(+0xf568)[0x55dd4c1d8568]
[fv-az99-305:11488] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7ff2b34290b3]
[fv-az99-305:11488] [ 9] plumed_master(+0xf79e)[0x55dd4c1d879e]
[fv-az99-305:11488] *** End of error message ***
</pre>
{% endraw %}
