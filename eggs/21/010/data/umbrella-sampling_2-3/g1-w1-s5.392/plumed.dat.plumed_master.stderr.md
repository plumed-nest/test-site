**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_2-3/g1-w1-s5.392/plumed.dat   
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
[fv-az99-305:09952] *** Process received signal ***
[fv-az99-305:09952] Signal: Aborted (6)
[fv-az99-305:09952] Signal code:  (-6)
[fv-az99-305:09952] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7febc1a12210]
[fv-az99-305:09952] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7febc1a1218b]
[fv-az99-305:09952] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7febc19f1859]
[fv-az99-305:09952] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7febc1c79951]
[fv-az99-305:09952] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7febc1c8547c]
[fv-az99-305:09952] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7febc1c854e7]
[fv-az99-305:09952] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7febc1c857ed]
[fv-az99-305:09952] [ 7] plumed_master(+0xf568)[0x5596ce90d568]
[fv-az99-305:09952] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7febc19f30b3]
[fv-az99-305:09952] [ 9] plumed_master(+0xf79e)[0x5596ce90d79e]
[fv-az99-305:09952] *** End of error message ***
</pre>
{% endraw %}
