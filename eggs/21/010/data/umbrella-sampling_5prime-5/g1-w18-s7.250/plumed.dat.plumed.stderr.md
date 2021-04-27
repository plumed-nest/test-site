**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_5prime-5/g1-w18-s7.250/plumed.dat   
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
[fv-az99-305:15825] *** Process received signal ***
[fv-az99-305:15825] Signal: Aborted (6)
[fv-az99-305:15825] Signal code:  (-6)
[fv-az99-305:15825] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fe237f2a210]
[fv-az99-305:15825] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fe237f2a18b]
[fv-az99-305:15825] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fe237f09859]
[fv-az99-305:15825] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fe238191951]
[fv-az99-305:15825] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fe23819d47c]
[fv-az99-305:15825] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fe23819d4e7]
[fv-az99-305:15825] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fe23819d799]
[fv-az99-305:15825] [ 7] plumed(+0xf47d)[0x55ef29df147d]
[fv-az99-305:15825] [ 8] plumed(+0x14004)[0x55ef29df6004]
[fv-az99-305:15825] [ 9] plumed(+0xf698)[0x55ef29df1698]
[fv-az99-305:15825] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fe237f0b0b3]
[fv-az99-305:15825] [11] plumed(+0xf76e)[0x55ef29df176e]
[fv-az99-305:15825] *** End of error message ***
</pre>
{% endraw %}
