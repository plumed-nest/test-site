**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_2prime-2/g1-w24-s8.338/plumed.dat   
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
[fv-az99-305:11211] *** Process received signal ***
[fv-az99-305:11211] Signal: Aborted (6)
[fv-az99-305:11211] Signal code:  (-6)
[fv-az99-305:11211] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fb792174210]
[fv-az99-305:11211] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fb79217418b]
[fv-az99-305:11211] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fb792153859]
[fv-az99-305:11211] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fb7923db951]
[fv-az99-305:11211] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fb7923e747c]
[fv-az99-305:11211] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fb7923e74e7]
[fv-az99-305:11211] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fb7923e7799]
[fv-az99-305:11211] [ 7] plumed(+0xf47d)[0x55de63e2c47d]
[fv-az99-305:11211] [ 8] plumed(+0x14004)[0x55de63e31004]
[fv-az99-305:11211] [ 9] plumed(+0xf698)[0x55de63e2c698]
[fv-az99-305:11211] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fb7921550b3]
[fv-az99-305:11211] [11] plumed(+0xf76e)[0x55de63e2c76e]
[fv-az99-305:11211] *** End of error message ***
</pre>
{% endraw %}
