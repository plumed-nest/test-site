**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_2-3/g1-w23-s9.425/plumed.dat   
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
[fv-az99-305:10359] *** Process received signal ***
[fv-az99-305:10359] Signal: Aborted (6)
[fv-az99-305:10359] Signal code:  (-6)
[fv-az99-305:10359] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f53b11c8210]
[fv-az99-305:10359] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f53b11c818b]
[fv-az99-305:10359] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f53b11a7859]
[fv-az99-305:10359] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f53b142f951]
[fv-az99-305:10359] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f53b143b47c]
[fv-az99-305:10359] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f53b143b4e7]
[fv-az99-305:10359] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f53b143b799]
[fv-az99-305:10359] [ 7] plumed(+0xf47d)[0x5564e005b47d]
[fv-az99-305:10359] [ 8] plumed(+0x14004)[0x5564e0060004]
[fv-az99-305:10359] [ 9] plumed(+0xf698)[0x5564e005b698]
[fv-az99-305:10359] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f53b11a90b3]
[fv-az99-305:10359] [11] plumed(+0xf76e)[0x5564e005b76e]
[fv-az99-305:10359] *** End of error message ***
</pre>
{% endraw %}
