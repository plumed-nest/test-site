**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_3-4/g202-w2-s4.632/plumed.dat   
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
[fv-az99-305:12560] *** Process received signal ***
[fv-az99-305:12560] Signal: Aborted (6)
[fv-az99-305:12560] Signal code:  (-6)
[fv-az99-305:12560] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f07a516a210]
[fv-az99-305:12560] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f07a516a18b]
[fv-az99-305:12560] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f07a5149859]
[fv-az99-305:12560] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f07a53d1951]
[fv-az99-305:12560] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f07a53dd47c]
[fv-az99-305:12560] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f07a53dd4e7]
[fv-az99-305:12560] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f07a53dd799]
[fv-az99-305:12560] [ 7] plumed(+0xf47d)[0x55f8af28a47d]
[fv-az99-305:12560] [ 8] plumed(+0x14004)[0x55f8af28f004]
[fv-az99-305:12560] [ 9] plumed(+0xf698)[0x55f8af28a698]
[fv-az99-305:12560] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f07a514b0b3]
[fv-az99-305:12560] [11] plumed(+0xf76e)[0x55f8af28a76e]
[fv-az99-305:12560] *** End of error message ***
</pre>
{% endraw %}
