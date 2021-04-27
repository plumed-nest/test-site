**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_5-6/g1-w2-s1.875/plumed.dat   
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
[fv-az99-305:14647] *** Process received signal ***
[fv-az99-305:14647] Signal: Aborted (6)
[fv-az99-305:14647] Signal code:  (-6)
[fv-az99-305:14647] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fe25a20f210]
[fv-az99-305:14647] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fe25a20f18b]
[fv-az99-305:14647] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fe25a1ee859]
[fv-az99-305:14647] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fe25a476951]
[fv-az99-305:14647] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fe25a48247c]
[fv-az99-305:14647] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fe25a4824e7]
[fv-az99-305:14647] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fe25a482799]
[fv-az99-305:14647] [ 7] plumed(+0xf47d)[0x564b1961c47d]
[fv-az99-305:14647] [ 8] plumed(+0x14004)[0x564b19621004]
[fv-az99-305:14647] [ 9] plumed(+0xf698)[0x564b1961c698]
[fv-az99-305:14647] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fe25a1f00b3]
[fv-az99-305:14647] [11] plumed(+0xf76e)[0x564b1961c76e]
[fv-az99-305:14647] *** End of error message ***
</pre>
{% endraw %}
