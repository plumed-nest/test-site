**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_3-4/g2-w13-s5.995/plumed.dat   
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
[fv-az99-305:11948] *** Process received signal ***
[fv-az99-305:11948] Signal: Aborted (6)
[fv-az99-305:11948] Signal code:  (-6)
[fv-az99-305:11948] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fde3a249210]
[fv-az99-305:11948] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fde3a24918b]
[fv-az99-305:11948] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fde3a228859]
[fv-az99-305:11948] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fde3a4b0951]
[fv-az99-305:11948] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fde3a4bc47c]
[fv-az99-305:11948] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fde3a4bc4e7]
[fv-az99-305:11948] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fde3a4bc799]
[fv-az99-305:11948] [ 7] plumed(+0xf47d)[0x563e544ae47d]
[fv-az99-305:11948] [ 8] plumed(+0x14004)[0x563e544b3004]
[fv-az99-305:11948] [ 9] plumed(+0xf698)[0x563e544ae698]
[fv-az99-305:11948] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fde3a22a0b3]
[fv-az99-305:11948] [11] plumed(+0xf76e)[0x563e544ae76e]
[fv-az99-305:11948] *** End of error message ***
</pre>
{% endraw %}
