**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_2-3/g1-w2-s5.575/plumed.dat   
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
[fv-az99-305:10262] *** Process received signal ***
[fv-az99-305:10262] Signal: Aborted (6)
[fv-az99-305:10262] Signal code:  (-6)
[fv-az99-305:10262] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fc27399d210]
[fv-az99-305:10262] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fc27399d18b]
[fv-az99-305:10262] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fc27397c859]
[fv-az99-305:10262] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fc273c04951]
[fv-az99-305:10262] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fc273c1047c]
[fv-az99-305:10262] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fc273c104e7]
[fv-az99-305:10262] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fc273c10799]
[fv-az99-305:10262] [ 7] plumed(+0xf47d)[0x55f006d2147d]
[fv-az99-305:10262] [ 8] plumed(+0x14004)[0x55f006d26004]
[fv-az99-305:10262] [ 9] plumed(+0xf698)[0x55f006d21698]
[fv-az99-305:10262] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fc27397e0b3]
[fv-az99-305:10262] [11] plumed(+0xf76e)[0x55f006d2176e]
[fv-az99-305:10262] *** End of error message ***
</pre>
{% endraw %}
