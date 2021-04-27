**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_3-4/g201-w1-s6.060/plumed.dat   
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
[fv-az99-305:12494] *** Process received signal ***
[fv-az99-305:12494] Signal: Aborted (6)
[fv-az99-305:12494] Signal code:  (-6)
[fv-az99-305:12494] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f88f5111210]
[fv-az99-305:12494] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f88f511118b]
[fv-az99-305:12494] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f88f50f0859]
[fv-az99-305:12494] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f88f5378951]
[fv-az99-305:12494] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f88f538447c]
[fv-az99-305:12494] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f88f53844e7]
[fv-az99-305:12494] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7f88f53847ed]
[fv-az99-305:12494] [ 7] plumed_master(+0xf568)[0x5605a4522568]
[fv-az99-305:12494] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f88f50f20b3]
[fv-az99-305:12494] [ 9] plumed_master(+0xf79e)[0x5605a452279e]
[fv-az99-305:12494] *** End of error message ***
</pre>
{% endraw %}
