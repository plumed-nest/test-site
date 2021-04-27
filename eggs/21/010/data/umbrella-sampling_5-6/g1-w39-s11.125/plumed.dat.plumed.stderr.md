**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_5-6/g1-w39-s11.125/plumed.dat   
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
[fv-az99-305:15160] *** Process received signal ***
[fv-az99-305:15160] Signal: Aborted (6)
[fv-az99-305:15160] Signal code:  (-6)
[fv-az99-305:15160] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f01c74bd210]
[fv-az99-305:15160] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f01c74bd18b]
[fv-az99-305:15160] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f01c749c859]
[fv-az99-305:15160] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f01c7724951]
[fv-az99-305:15160] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f01c773047c]
[fv-az99-305:15160] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f01c77304e7]
[fv-az99-305:15160] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f01c7730799]
[fv-az99-305:15160] [ 7] plumed(+0xf47d)[0x563b8b7b647d]
[fv-az99-305:15160] [ 8] plumed(+0x14004)[0x563b8b7bb004]
[fv-az99-305:15160] [ 9] plumed(+0xf698)[0x563b8b7b6698]
[fv-az99-305:15160] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f01c749e0b3]
[fv-az99-305:15160] [11] plumed(+0xf76e)[0x563b8b7b676e]
[fv-az99-305:15160] *** End of error message ***
</pre>
{% endraw %}
