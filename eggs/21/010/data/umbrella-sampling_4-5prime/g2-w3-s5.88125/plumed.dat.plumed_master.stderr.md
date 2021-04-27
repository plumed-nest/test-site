**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_4-5prime/g2-w3-s5.88125/plumed.dat   
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
[fv-az99-305:14312] *** Process received signal ***
[fv-az99-305:14312] Signal: Aborted (6)
[fv-az99-305:14312] Signal code:  (-6)
[fv-az99-305:14312] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f30e8aa0210]
[fv-az99-305:14312] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f30e8aa018b]
[fv-az99-305:14312] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f30e8a7f859]
[fv-az99-305:14312] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f30e8d07951]
[fv-az99-305:14312] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f30e8d1347c]
[fv-az99-305:14312] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f30e8d134e7]
[fv-az99-305:14312] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7f30e8d137ed]
[fv-az99-305:14312] [ 7] plumed_master(+0xf568)[0x559a3cb80568]
[fv-az99-305:14312] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f30e8a810b3]
[fv-az99-305:14312] [ 9] plumed_master(+0xf79e)[0x559a3cb8079e]
[fv-az99-305:14312] *** End of error message ***
</pre>
{% endraw %}
