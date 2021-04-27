**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_4-5prime/g4-w1-s9.9385/plumed.dat   
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
[fv-az99-305:14352] *** Process received signal ***
[fv-az99-305:14352] Signal: Aborted (6)
[fv-az99-305:14352] Signal code:  (-6)
[fv-az99-305:14352] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fa63de8d210]
[fv-az99-305:14352] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fa63de8d18b]
[fv-az99-305:14352] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fa63de6c859]
[fv-az99-305:14352] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fa63e0f4951]
[fv-az99-305:14352] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fa63e10047c]
[fv-az99-305:14352] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fa63e1004e7]
[fv-az99-305:14352] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fa63e100799]
[fv-az99-305:14352] [ 7] plumed(+0xf47d)[0x55be5eb3d47d]
[fv-az99-305:14352] [ 8] plumed(+0x14004)[0x55be5eb42004]
[fv-az99-305:14352] [ 9] plumed(+0xf698)[0x55be5eb3d698]
[fv-az99-305:14352] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fa63de6e0b3]
[fv-az99-305:14352] [11] plumed(+0xf76e)[0x55be5eb3d76e]
[fv-az99-305:14352] *** End of error message ***
</pre>
{% endraw %}
