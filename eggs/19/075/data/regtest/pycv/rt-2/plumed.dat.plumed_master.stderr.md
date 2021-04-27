**Project ID:** [plumID:19.075]({{ '/' | absolute_url }}eggs/19/075/)  
Stderr for source:  regtest/pycv/rt-2/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:704, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: PYTHONCV LABEL=cv1 ATOMS=1,4 IMPORT=distcv FUNCTION=cv
Maybe a missing space or a typo?
[fv-az99-305:30333] *** Process received signal ***
[fv-az99-305:30333] Signal: Aborted (6)
[fv-az99-305:30333] Signal code:  (-6)
[fv-az99-305:30333] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f8132b2b210]
[fv-az99-305:30333] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f8132b2b18b]
[fv-az99-305:30333] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f8132b0a859]
[fv-az99-305:30333] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f8132d92951]
[fv-az99-305:30333] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f8132d9e47c]
[fv-az99-305:30333] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f8132d9e4e7]
[fv-az99-305:30333] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7f8132d9e7ed]
[fv-az99-305:30333] [ 7] plumed_master(+0xf568)[0x560300523568]
[fv-az99-305:30333] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f8132b0c0b3]
[fv-az99-305:30333] [ 9] plumed_master(+0xf79e)[0x56030052379e]
[fv-az99-305:30333] *** End of error message ***
</pre>
{% endraw %}
