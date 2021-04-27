**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_4-5prime/g1-w18-s4.554/plumed.dat   
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
[fv-az99-305:13006] *** Process received signal ***
[fv-az99-305:13006] Signal: Aborted (6)
[fv-az99-305:13006] Signal code:  (-6)
[fv-az99-305:13006] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f3432979210]
[fv-az99-305:13006] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f343297918b]
[fv-az99-305:13006] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f3432958859]
[fv-az99-305:13006] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f3432be0951]
[fv-az99-305:13006] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f3432bec47c]
[fv-az99-305:13006] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f3432bec4e7]
[fv-az99-305:13006] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f3432bec799]
[fv-az99-305:13006] [ 7] plumed(+0xf47d)[0x55bda805447d]
[fv-az99-305:13006] [ 8] plumed(+0x14004)[0x55bda8059004]
[fv-az99-305:13006] [ 9] plumed(+0xf698)[0x55bda8054698]
[fv-az99-305:13006] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f343295a0b3]
[fv-az99-305:13006] [11] plumed(+0xf76e)[0x55bda805476e]
[fv-az99-305:13006] *** End of error message ***
</pre>
{% endraw %}
