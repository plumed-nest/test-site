**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w25-s6.492/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:706, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: HILLS RESTART HEIGHT 0.000 W_STRIDE 50
Maybe a missing space or a typo?
[fv-az99-305:08958] *** Process received signal ***
[fv-az99-305:08958] Signal: Aborted (6)
[fv-az99-305:08958] Signal code:  (-6)
[fv-az99-305:08958] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f1e29b93210]
[fv-az99-305:08958] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f1e29b9318b]
[fv-az99-305:08958] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f1e29b72859]
[fv-az99-305:08958] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f1e29dfa951]
[fv-az99-305:08958] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f1e29e0647c]
[fv-az99-305:08958] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f1e29e064e7]
[fv-az99-305:08958] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f1e29e06799]
[fv-az99-305:08958] [ 7] plumed(+0xf47d)[0x5610a41f547d]
[fv-az99-305:08958] [ 8] plumed(+0x14004)[0x5610a41fa004]
[fv-az99-305:08958] [ 9] plumed(+0xf698)[0x5610a41f5698]
[fv-az99-305:08958] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f1e29b740b3]
[fv-az99-305:08958] [11] plumed(+0xf76e)[0x5610a41f576e]
[fv-az99-305:08958] *** End of error message ***
</pre>
{% endraw %}
