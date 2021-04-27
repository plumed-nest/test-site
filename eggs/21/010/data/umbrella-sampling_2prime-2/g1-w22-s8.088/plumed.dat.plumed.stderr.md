**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_2prime-2/g1-w22-s8.088/plumed.dat   
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
[fv-az99-305:11162] *** Process received signal ***
[fv-az99-305:11162] Signal: Aborted (6)
[fv-az99-305:11162] Signal code:  (-6)
[fv-az99-305:11162] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f870b24c210]
[fv-az99-305:11162] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f870b24c18b]
[fv-az99-305:11162] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f870b22b859]
[fv-az99-305:11162] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f870b4b3951]
[fv-az99-305:11162] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f870b4bf47c]
[fv-az99-305:11162] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f870b4bf4e7]
[fv-az99-305:11162] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f870b4bf799]
[fv-az99-305:11162] [ 7] plumed(+0xf47d)[0x555ce0ac747d]
[fv-az99-305:11162] [ 8] plumed(+0x14004)[0x555ce0acc004]
[fv-az99-305:11162] [ 9] plumed(+0xf698)[0x555ce0ac7698]
[fv-az99-305:11162] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f870b22d0b3]
[fv-az99-305:11162] [11] plumed(+0xf76e)[0x555ce0ac776e]
[fv-az99-305:11162] *** End of error message ***
</pre>
{% endraw %}
