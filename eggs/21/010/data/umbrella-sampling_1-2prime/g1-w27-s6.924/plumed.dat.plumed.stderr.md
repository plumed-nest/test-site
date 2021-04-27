**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w27-s6.924/plumed.dat   
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
[fv-az99-305:09008] *** Process received signal ***
[fv-az99-305:09008] Signal: Aborted (6)
[fv-az99-305:09008] Signal code:  (-6)
[fv-az99-305:09008] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f4b7f2da210]
[fv-az99-305:09008] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f4b7f2da18b]
[fv-az99-305:09008] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f4b7f2b9859]
[fv-az99-305:09008] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f4b7f541951]
[fv-az99-305:09008] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f4b7f54d47c]
[fv-az99-305:09008] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f4b7f54d4e7]
[fv-az99-305:09008] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f4b7f54d799]
[fv-az99-305:09008] [ 7] plumed(+0xf47d)[0x555f091ff47d]
[fv-az99-305:09008] [ 8] plumed(+0x14004)[0x555f09204004]
[fv-az99-305:09008] [ 9] plumed(+0xf698)[0x555f091ff698]
[fv-az99-305:09008] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f4b7f2bb0b3]
[fv-az99-305:09008] [11] plumed(+0xf76e)[0x555f091ff76e]
[fv-az99-305:09008] *** End of error message ***
</pre>
{% endraw %}
