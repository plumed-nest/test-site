**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_2-3/g1-w21-s9.058/plumed.dat   
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
[fv-az99-305:10310] *** Process received signal ***
[fv-az99-305:10310] Signal: Aborted (6)
[fv-az99-305:10310] Signal code:  (-6)
[fv-az99-305:10310] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7ff8f8cba210]
[fv-az99-305:10310] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7ff8f8cba18b]
[fv-az99-305:10310] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7ff8f8c99859]
[fv-az99-305:10310] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7ff8f8f21951]
[fv-az99-305:10310] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7ff8f8f2d47c]
[fv-az99-305:10310] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7ff8f8f2d4e7]
[fv-az99-305:10310] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7ff8f8f2d799]
[fv-az99-305:10310] [ 7] plumed(+0xf47d)[0x55fa6dc1147d]
[fv-az99-305:10310] [ 8] plumed(+0x14004)[0x55fa6dc16004]
[fv-az99-305:10310] [ 9] plumed(+0xf698)[0x55fa6dc11698]
[fv-az99-305:10310] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7ff8f8c9b0b3]
[fv-az99-305:10310] [11] plumed(+0xf76e)[0x55fa6dc1176e]
[fv-az99-305:10310] *** End of error message ***
</pre>
{% endraw %}
