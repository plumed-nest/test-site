**Project ID:** [plumID:19.075]({{ '/' | absolute_url }}eggs/19/075/)  
Stderr for source:  regtest/pycv/rt-1/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:704, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: PYTHONCV LABEL=cv1 ATOMS=1,4 IMPORT=pycv FUNCTION=cv1
Maybe a missing space or a typo?
[fv-az99-305:30308] *** Process received signal ***
[fv-az99-305:30308] Signal: Aborted (6)
[fv-az99-305:30308] Signal code:  (-6)
[fv-az99-305:30308] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f2bf2f37210]
[fv-az99-305:30308] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f2bf2f3718b]
[fv-az99-305:30308] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f2bf2f16859]
[fv-az99-305:30308] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f2bf319e951]
[fv-az99-305:30308] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f2bf31aa47c]
[fv-az99-305:30308] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f2bf31aa4e7]
[fv-az99-305:30308] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7f2bf31aa7ed]
[fv-az99-305:30308] [ 7] plumed_master(+0xf568)[0x5637c9813568]
[fv-az99-305:30308] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f2bf2f180b3]
[fv-az99-305:30308] [ 9] plumed_master(+0xf79e)[0x5637c981379e]
[fv-az99-305:30308] *** End of error message ***
</pre>
{% endraw %}
