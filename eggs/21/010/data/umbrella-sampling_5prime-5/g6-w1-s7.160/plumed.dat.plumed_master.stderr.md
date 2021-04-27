**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_5prime-5/g6-w1-s7.160/plumed.dat   
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
[fv-az99-305:16446] *** Process received signal ***
[fv-az99-305:16446] Signal: Aborted (6)
[fv-az99-305:16446] Signal code:  (-6)
[fv-az99-305:16446] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7faa5dc4d210]
[fv-az99-305:16446] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7faa5dc4d18b]
[fv-az99-305:16446] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7faa5dc2c859]
[fv-az99-305:16446] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7faa5deb4951]
[fv-az99-305:16446] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7faa5dec047c]
[fv-az99-305:16446] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7faa5dec04e7]
[fv-az99-305:16446] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7faa5dec07ed]
[fv-az99-305:16446] [ 7] plumed_master(+0xf568)[0x562a5f6c5568]
[fv-az99-305:16446] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7faa5dc2e0b3]
[fv-az99-305:16446] [ 9] plumed_master(+0xf79e)[0x562a5f6c579e]
[fv-az99-305:16446] *** End of error message ***
</pre>
{% endraw %}
