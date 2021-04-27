**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_2prime-2/g4-w5-s10.427/plumed.dat   
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
[fv-az99-305:11750] *** Process received signal ***
[fv-az99-305:11750] Signal: Aborted (6)
[fv-az99-305:11750] Signal code:  (-6)
[fv-az99-305:11750] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f3c4d9e0210]
[fv-az99-305:11750] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f3c4d9e018b]
[fv-az99-305:11750] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f3c4d9bf859]
[fv-az99-305:11750] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f3c4dc47951]
[fv-az99-305:11750] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f3c4dc5347c]
[fv-az99-305:11750] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f3c4dc534e7]
[fv-az99-305:11750] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f3c4dc53799]
[fv-az99-305:11750] [ 7] plumed(+0xf47d)[0x558e2e7b547d]
[fv-az99-305:11750] [ 8] plumed(+0x14004)[0x558e2e7ba004]
[fv-az99-305:11750] [ 9] plumed(+0xf698)[0x558e2e7b5698]
[fv-az99-305:11750] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f3c4d9c10b3]
[fv-az99-305:11750] [11] plumed(+0xf76e)[0x558e2e7b576e]
[fv-az99-305:11750] *** End of error message ***
</pre>
{% endraw %}
