**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_5-6/g1-w25-s7.625/plumed.dat   
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
[fv-az99-305:14802] *** Process received signal ***
[fv-az99-305:14802] Signal: Aborted (6)
[fv-az99-305:14802] Signal code:  (-6)
[fv-az99-305:14802] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fcf81909210]
[fv-az99-305:14802] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fcf8190918b]
[fv-az99-305:14802] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fcf818e8859]
[fv-az99-305:14802] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fcf81b70951]
[fv-az99-305:14802] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fcf81b7c47c]
[fv-az99-305:14802] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fcf81b7c4e7]
[fv-az99-305:14802] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7fcf81b7c7ed]
[fv-az99-305:14802] [ 7] plumed_master(+0xf568)[0x55dcea483568]
[fv-az99-305:14802] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fcf818ea0b3]
[fv-az99-305:14802] [ 9] plumed_master(+0xf79e)[0x55dcea48379e]
[fv-az99-305:14802] *** End of error message ***
</pre>
{% endraw %}
