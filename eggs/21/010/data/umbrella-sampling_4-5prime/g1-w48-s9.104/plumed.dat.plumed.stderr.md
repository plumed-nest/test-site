**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_4-5prime/g1-w48-s9.104/plumed.dat   
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
[fv-az99-305:13813] *** Process received signal ***
[fv-az99-305:13813] Signal: Aborted (6)
[fv-az99-305:13813] Signal code:  (-6)
[fv-az99-305:13813] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fe2621ba210]
[fv-az99-305:13813] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fe2621ba18b]
[fv-az99-305:13813] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fe262199859]
[fv-az99-305:13813] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fe262421951]
[fv-az99-305:13813] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fe26242d47c]
[fv-az99-305:13813] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fe26242d4e7]
[fv-az99-305:13813] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fe26242d799]
[fv-az99-305:13813] [ 7] plumed(+0xf47d)[0x55d00c9f747d]
[fv-az99-305:13813] [ 8] plumed(+0x14004)[0x55d00c9fc004]
[fv-az99-305:13813] [ 9] plumed(+0xf698)[0x55d00c9f7698]
[fv-az99-305:13813] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fe26219b0b3]
[fv-az99-305:13813] [11] plumed(+0xf76e)[0x55d00c9f776e]
[fv-az99-305:13813] *** End of error message ***
</pre>
{% endraw %}
