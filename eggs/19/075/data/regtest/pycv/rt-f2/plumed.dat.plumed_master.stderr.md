**Project ID:** [plumID:19.075]({{ '/' | absolute_url }}eggs/19/075/)  
Stderr for source:  regtest/pycv/rt-f2/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:704, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: PYTHONFUNCTION LABEL=cc1 ARG=t1,t2,t3 IMPORT=pythonfunction FUNCTION=cc1 PERIODIC=NO
Maybe a missing space or a typo?
[fv-az99-305:30406] *** Process received signal ***
[fv-az99-305:30406] Signal: Aborted (6)
[fv-az99-305:30406] Signal code:  (-6)
[fv-az99-305:30406] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f908ae9f210]
[fv-az99-305:30406] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f908ae9f18b]
[fv-az99-305:30406] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f908ae7e859]
[fv-az99-305:30406] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f908b106951]
[fv-az99-305:30406] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f908b11247c]
[fv-az99-305:30406] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f908b1124e7]
[fv-az99-305:30406] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7f908b1127ed]
[fv-az99-305:30406] [ 7] plumed_master(+0xf568)[0x55fb948a3568]
[fv-az99-305:30406] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f908ae800b3]
[fv-az99-305:30406] [ 9] plumed_master(+0xf79e)[0x55fb948a379e]
[fv-az99-305:30406] *** End of error message ***
</pre>
{% endraw %}
