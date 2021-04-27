**Project ID:** [plumID:19.075]({{ '/' | absolute_url }}eggs/19/075/)  
Stderr for source:  regtest/pycv/rt-jax3/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:704, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: PYTHONCV LABEL=r ATOMS=1,2,3 IMPORT=curvature FUNCTION=r
Maybe a missing space or a typo?
[fv-az99-305:30480] *** Process received signal ***
[fv-az99-305:30480] Signal: Aborted (6)
[fv-az99-305:30480] Signal code:  (-6)
[fv-az99-305:30480] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fd69d351210]
[fv-az99-305:30480] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fd69d35118b]
[fv-az99-305:30480] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fd69d330859]
[fv-az99-305:30480] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fd69d5b8951]
[fv-az99-305:30480] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fd69d5c447c]
[fv-az99-305:30480] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fd69d5c44e7]
[fv-az99-305:30480] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7fd69d5c47ed]
[fv-az99-305:30480] [ 7] plumed_master(+0xf568)[0x5644a59bb568]
[fv-az99-305:30480] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fd69d3320b3]
[fv-az99-305:30480] [ 9] plumed_master(+0xf79e)[0x5644a59bb79e]
[fv-az99-305:30480] *** End of error message ***
</pre>
{% endraw %}
