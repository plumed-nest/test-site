**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_2-3/g1-w17-s8.325/plumed.dat   
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
[fv-az99-305:10139] *** Process received signal ***
[fv-az99-305:10139] Signal: Aborted (6)
[fv-az99-305:10139] Signal code:  (-6)
[fv-az99-305:10139] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fb67f04d210]
[fv-az99-305:10139] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fb67f04d18b]
[fv-az99-305:10139] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fb67f02c859]
[fv-az99-305:10139] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fb67f2b4951]
[fv-az99-305:10139] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fb67f2c047c]
[fv-az99-305:10139] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fb67f2c04e7]
[fv-az99-305:10139] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fb67f2c0799]
[fv-az99-305:10139] [ 7] plumed(+0xf47d)[0x5562cd41847d]
[fv-az99-305:10139] [ 8] plumed(+0x14004)[0x5562cd41d004]
[fv-az99-305:10139] [ 9] plumed(+0xf698)[0x5562cd418698]
[fv-az99-305:10139] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fb67f02e0b3]
[fv-az99-305:10139] [11] plumed(+0xf76e)[0x5562cd41876e]
[fv-az99-305:10139] *** End of error message ***
</pre>
{% endraw %}
