**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_5-6/g1-w40-s11.375/plumed.dat   
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
[fv-az99-305:15217] *** Process received signal ***
[fv-az99-305:15217] Signal: Aborted (6)
[fv-az99-305:15217] Signal code:  (-6)
[fv-az99-305:15217] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f57550ae210]
[fv-az99-305:15217] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f57550ae18b]
[fv-az99-305:15217] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f575508d859]
[fv-az99-305:15217] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f5755315951]
[fv-az99-305:15217] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f575532147c]
[fv-az99-305:15217] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f57553214e7]
[fv-az99-305:15217] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7f57553217ed]
[fv-az99-305:15217] [ 7] plumed_master(+0xf568)[0x5583b4ae5568]
[fv-az99-305:15217] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f575508f0b3]
[fv-az99-305:15217] [ 9] plumed_master(+0xf79e)[0x5583b4ae579e]
[fv-az99-305:15217] *** End of error message ***
</pre>
{% endraw %}
