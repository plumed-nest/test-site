**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_3-4/g6-w1-s6.3845/plumed.dat   
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
[fv-az99-305:12710] *** Process received signal ***
[fv-az99-305:12710] Signal: Aborted (6)
[fv-az99-305:12710] Signal code:  (-6)
[fv-az99-305:12710] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f86cc14c210]
[fv-az99-305:12710] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f86cc14c18b]
[fv-az99-305:12710] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f86cc12b859]
[fv-az99-305:12710] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f86cc3b3951]
[fv-az99-305:12710] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f86cc3bf47c]
[fv-az99-305:12710] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f86cc3bf4e7]
[fv-az99-305:12710] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f86cc3bf799]
[fv-az99-305:12710] [ 7] plumed(+0xf47d)[0x559d9c41347d]
[fv-az99-305:12710] [ 8] plumed(+0x14004)[0x559d9c418004]
[fv-az99-305:12710] [ 9] plumed(+0xf698)[0x559d9c413698]
[fv-az99-305:12710] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f86cc12d0b3]
[fv-az99-305:12710] [11] plumed(+0xf76e)[0x559d9c41376e]
[fv-az99-305:12710] *** End of error message ***
</pre>
{% endraw %}
