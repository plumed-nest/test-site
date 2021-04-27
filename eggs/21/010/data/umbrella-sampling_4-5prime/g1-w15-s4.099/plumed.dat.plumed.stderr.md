**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_4-5prime/g1-w15-s4.099/plumed.dat   
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
[fv-az99-305:12933] *** Process received signal ***
[fv-az99-305:12933] Signal: Aborted (6)
[fv-az99-305:12933] Signal code:  (-6)
[fv-az99-305:12933] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f9e738ff210]
[fv-az99-305:12933] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f9e738ff18b]
[fv-az99-305:12933] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f9e738de859]
[fv-az99-305:12933] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f9e73b66951]
[fv-az99-305:12933] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f9e73b7247c]
[fv-az99-305:12933] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f9e73b724e7]
[fv-az99-305:12933] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f9e73b72799]
[fv-az99-305:12933] [ 7] plumed(+0xf47d)[0x560b2785c47d]
[fv-az99-305:12933] [ 8] plumed(+0x14004)[0x560b27861004]
[fv-az99-305:12933] [ 9] plumed(+0xf698)[0x560b2785c698]
[fv-az99-305:12933] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f9e738e00b3]
[fv-az99-305:12933] [11] plumed(+0xf76e)[0x560b2785c76e]
[fv-az99-305:12933] *** End of error message ***
</pre>
{% endraw %}
