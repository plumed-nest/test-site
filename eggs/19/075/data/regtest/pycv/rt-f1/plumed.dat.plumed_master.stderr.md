**Project ID:** [plumID:19.075]({{ '/' | absolute_url }}eggs/19/075/)  
Stderr for source:  regtest/pycv/rt-f1/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:704, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: PYTHONFUNCTION LABEL=dAB2 ARG=dAB IMPORT=pythonfunction FUNCTION=square PERIODIC=NO
Maybe a missing space or a typo?
[fv-az99-305:30382] *** Process received signal ***
[fv-az99-305:30382] Signal: Aborted (6)
[fv-az99-305:30382] Signal code:  (-6)
[fv-az99-305:30382] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f07a8f87210]
[fv-az99-305:30382] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f07a8f8718b]
[fv-az99-305:30382] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f07a8f66859]
[fv-az99-305:30382] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f07a91ee951]
[fv-az99-305:30382] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f07a91fa47c]
[fv-az99-305:30382] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f07a91fa4e7]
[fv-az99-305:30382] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7f07a91fa7ed]
[fv-az99-305:30382] [ 7] plumed_master(+0xf568)[0x5578abae0568]
[fv-az99-305:30382] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f07a8f680b3]
[fv-az99-305:30382] [ 9] plumed_master(+0xf79e)[0x5578abae079e]
[fv-az99-305:30382] *** End of error message ***
</pre>
{% endraw %}
