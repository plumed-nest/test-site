**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_2-3/g1-w12-s7.408/plumed.dat   
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
[fv-az99-305:10018] *** Process received signal ***
[fv-az99-305:10018] Signal: Aborted (6)
[fv-az99-305:10018] Signal code:  (-6)
[fv-az99-305:10018] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f4113315210]
[fv-az99-305:10018] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f411331518b]
[fv-az99-305:10018] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f41132f4859]
[fv-az99-305:10018] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f411357c951]
[fv-az99-305:10018] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f411358847c]
[fv-az99-305:10018] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f41135884e7]
[fv-az99-305:10018] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f4113588799]
[fv-az99-305:10018] [ 7] plumed(+0xf47d)[0x562f8aba047d]
[fv-az99-305:10018] [ 8] plumed(+0x14004)[0x562f8aba5004]
[fv-az99-305:10018] [ 9] plumed(+0xf698)[0x562f8aba0698]
[fv-az99-305:10018] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f41132f60b3]
[fv-az99-305:10018] [11] plumed(+0xf76e)[0x562f8aba076e]
[fv-az99-305:10018] *** End of error message ***
</pre>
{% endraw %}
