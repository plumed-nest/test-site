**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_4-5prime/g4-w1-s9.9385/plumed.dat   
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
[fv-az99-305:14360] *** Process received signal ***
[fv-az99-305:14360] Signal: Aborted (6)
[fv-az99-305:14360] Signal code:  (-6)
[fv-az99-305:14360] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f5fb195a210]
[fv-az99-305:14360] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f5fb195a18b]
[fv-az99-305:14360] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f5fb1939859]
[fv-az99-305:14360] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f5fb1bc1951]
[fv-az99-305:14360] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f5fb1bcd47c]
[fv-az99-305:14360] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f5fb1bcd4e7]
[fv-az99-305:14360] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7f5fb1bcd7ed]
[fv-az99-305:14360] [ 7] plumed_master(+0xf568)[0x563e6f003568]
[fv-az99-305:14360] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f5fb193b0b3]
[fv-az99-305:14360] [ 9] plumed_master(+0xf79e)[0x563e6f00379e]
[fv-az99-305:14360] *** End of error message ***
</pre>
{% endraw %}
