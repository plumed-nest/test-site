**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_4-5prime/g1-w25-s5.616/plumed.dat   
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
[fv-az99-305:13203] *** Process received signal ***
[fv-az99-305:13203] Signal: Aborted (6)
[fv-az99-305:13203] Signal code:  (-6)
[fv-az99-305:13203] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7faff66bb210]
[fv-az99-305:13203] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7faff66bb18b]
[fv-az99-305:13203] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7faff669a859]
[fv-az99-305:13203] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7faff6922951]
[fv-az99-305:13203] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7faff692e47c]
[fv-az99-305:13203] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7faff692e4e7]
[fv-az99-305:13203] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7faff692e799]
[fv-az99-305:13203] [ 7] plumed(+0xf47d)[0x556e4c86247d]
[fv-az99-305:13203] [ 8] plumed(+0x14004)[0x556e4c867004]
[fv-az99-305:13203] [ 9] plumed(+0xf698)[0x556e4c862698]
[fv-az99-305:13203] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7faff669c0b3]
[fv-az99-305:13203] [11] plumed(+0xf76e)[0x556e4c86276e]
[fv-az99-305:13203] *** End of error message ***
</pre>
{% endraw %}
