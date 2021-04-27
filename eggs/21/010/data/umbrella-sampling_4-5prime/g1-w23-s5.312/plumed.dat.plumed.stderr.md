**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_4-5prime/g1-w23-s5.312/plumed.dat   
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
[fv-az99-305:13153] *** Process received signal ***
[fv-az99-305:13153] Signal: Aborted (6)
[fv-az99-305:13153] Signal code:  (-6)
[fv-az99-305:13153] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f7bc5d5c210]
[fv-az99-305:13153] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f7bc5d5c18b]
[fv-az99-305:13153] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f7bc5d3b859]
[fv-az99-305:13153] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f7bc5fc3951]
[fv-az99-305:13153] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f7bc5fcf47c]
[fv-az99-305:13153] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f7bc5fcf4e7]
[fv-az99-305:13153] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f7bc5fcf799]
[fv-az99-305:13153] [ 7] plumed(+0xf47d)[0x562a2343547d]
[fv-az99-305:13153] [ 8] plumed(+0x14004)[0x562a2343a004]
[fv-az99-305:13153] [ 9] plumed(+0xf698)[0x562a23435698]
[fv-az99-305:13153] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f7bc5d3d0b3]
[fv-az99-305:13153] [11] plumed(+0xf76e)[0x562a2343576e]
[fv-az99-305:13153] *** End of error message ***
</pre>
{% endraw %}
