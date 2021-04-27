**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w26-s6.708/plumed.dat   
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
[fv-az99-305:08983] *** Process received signal ***
[fv-az99-305:08983] Signal: Aborted (6)
[fv-az99-305:08983] Signal code:  (-6)
[fv-az99-305:08983] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f3366a94210]
[fv-az99-305:08983] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f3366a9418b]
[fv-az99-305:08983] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f3366a73859]
[fv-az99-305:08983] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f3366cfb951]
[fv-az99-305:08983] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f3366d0747c]
[fv-az99-305:08983] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f3366d074e7]
[fv-az99-305:08983] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f3366d07799]
[fv-az99-305:08983] [ 7] plumed(+0xf47d)[0x55ea8ed3047d]
[fv-az99-305:08983] [ 8] plumed(+0x14004)[0x55ea8ed35004]
[fv-az99-305:08983] [ 9] plumed(+0xf698)[0x55ea8ed30698]
[fv-az99-305:08983] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f3366a750b3]
[fv-az99-305:08983] [11] plumed(+0xf76e)[0x55ea8ed3076e]
[fv-az99-305:08983] *** End of error message ***
</pre>
{% endraw %}
