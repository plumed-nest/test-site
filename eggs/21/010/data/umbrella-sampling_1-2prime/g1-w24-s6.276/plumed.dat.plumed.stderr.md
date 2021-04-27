**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w24-s6.276/plumed.dat   
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
[fv-az99-305:08934] *** Process received signal ***
[fv-az99-305:08934] Signal: Aborted (6)
[fv-az99-305:08934] Signal code:  (-6)
[fv-az99-305:08934] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fe1ae2d7210]
[fv-az99-305:08934] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fe1ae2d718b]
[fv-az99-305:08934] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fe1ae2b6859]
[fv-az99-305:08934] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fe1ae53e951]
[fv-az99-305:08934] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fe1ae54a47c]
[fv-az99-305:08934] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fe1ae54a4e7]
[fv-az99-305:08934] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fe1ae54a799]
[fv-az99-305:08934] [ 7] plumed(+0xf47d)[0x562752f6547d]
[fv-az99-305:08934] [ 8] plumed(+0x14004)[0x562752f6a004]
[fv-az99-305:08934] [ 9] plumed(+0xf698)[0x562752f65698]
[fv-az99-305:08934] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fe1ae2b80b3]
[fv-az99-305:08934] [11] plumed(+0xf76e)[0x562752f6576e]
[fv-az99-305:08934] *** End of error message ***
</pre>
{% endraw %}
