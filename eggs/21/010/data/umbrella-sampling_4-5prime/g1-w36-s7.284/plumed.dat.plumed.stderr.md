**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_4-5prime/g1-w36-s7.284/plumed.dat   
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
[fv-az99-305:13496] *** Process received signal ***
[fv-az99-305:13496] Signal: Aborted (6)
[fv-az99-305:13496] Signal code:  (-6)
[fv-az99-305:13496] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fd1c450f210]
[fv-az99-305:13496] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fd1c450f18b]
[fv-az99-305:13496] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fd1c44ee859]
[fv-az99-305:13496] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fd1c4776951]
[fv-az99-305:13496] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fd1c478247c]
[fv-az99-305:13496] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fd1c47824e7]
[fv-az99-305:13496] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fd1c4782799]
[fv-az99-305:13496] [ 7] plumed(+0xf47d)[0x5574eaa7147d]
[fv-az99-305:13496] [ 8] plumed(+0x14004)[0x5574eaa76004]
[fv-az99-305:13496] [ 9] plumed(+0xf698)[0x5574eaa71698]
[fv-az99-305:13496] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fd1c44f00b3]
[fv-az99-305:13496] [11] plumed(+0xf76e)[0x5574eaa7176e]
[fv-az99-305:13496] *** End of error message ***
</pre>
{% endraw %}
