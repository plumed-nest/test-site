**Project ID:** [plumID:19.075]({{ '/' | absolute_url }}eggs/19/075/)  
Stderr for source:  regtest/pycv/rt-multi-1/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:704, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: PYTHONCV LABEL=cv1 ATOMS=1,3,4 IMPORT=distcv FUNCTION=cv COMPONENTS=d12,d13
Maybe a missing space or a typo?
[fv-az99-305:30505] *** Process received signal ***
[fv-az99-305:30505] Signal: Aborted (6)
[fv-az99-305:30505] Signal code:  (-6)
[fv-az99-305:30505] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f2115ef3210]
[fv-az99-305:30505] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f2115ef318b]
[fv-az99-305:30505] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f2115ed2859]
[fv-az99-305:30505] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f211615a951]
[fv-az99-305:30505] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f211616647c]
[fv-az99-305:30505] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f21161664e7]
[fv-az99-305:30505] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7f21161667ed]
[fv-az99-305:30505] [ 7] plumed_master(+0xf568)[0x55fb84614568]
[fv-az99-305:30505] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f2115ed40b3]
[fv-az99-305:30505] [ 9] plumed_master(+0xf79e)[0x55fb8461479e]
[fv-az99-305:30505] *** End of error message ***
</pre>
{% endraw %}
