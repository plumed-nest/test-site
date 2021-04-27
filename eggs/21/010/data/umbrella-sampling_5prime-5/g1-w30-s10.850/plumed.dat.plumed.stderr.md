**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_5prime-5/g1-w30-s10.850/plumed.dat   
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
[fv-az99-305:16167] *** Process received signal ***
[fv-az99-305:16167] Signal: Aborted (6)
[fv-az99-305:16167] Signal code:  (-6)
[fv-az99-305:16167] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7ff0c3c79210]
[fv-az99-305:16167] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7ff0c3c7918b]
[fv-az99-305:16167] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7ff0c3c58859]
[fv-az99-305:16167] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7ff0c3ee0951]
[fv-az99-305:16167] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7ff0c3eec47c]
[fv-az99-305:16167] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7ff0c3eec4e7]
[fv-az99-305:16167] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7ff0c3eec799]
[fv-az99-305:16167] [ 7] plumed(+0xf47d)[0x55c4e553547d]
[fv-az99-305:16167] [ 8] plumed(+0x14004)[0x55c4e553a004]
[fv-az99-305:16167] [ 9] plumed(+0xf698)[0x55c4e5535698]
[fv-az99-305:16167] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7ff0c3c5a0b3]
[fv-az99-305:16167] [11] plumed(+0xf76e)[0x55c4e553576e]
[fv-az99-305:16167] *** End of error message ***
</pre>
{% endraw %}
