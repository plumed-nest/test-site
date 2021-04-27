**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_5-6/g1-w17-s5.625/plumed.dat   
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
[fv-az99-305:14575] *** Process received signal ***
[fv-az99-305:14575] Signal: Aborted (6)
[fv-az99-305:14575] Signal code:  (-6)
[fv-az99-305:14575] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f39169d0210]
[fv-az99-305:14575] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f39169d018b]
[fv-az99-305:14575] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f39169af859]
[fv-az99-305:14575] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f3916c37951]
[fv-az99-305:14575] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f3916c4347c]
[fv-az99-305:14575] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f3916c434e7]
[fv-az99-305:14575] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f3916c43799]
[fv-az99-305:14575] [ 7] plumed(+0xf47d)[0x555cb970147d]
[fv-az99-305:14575] [ 8] plumed(+0x14004)[0x555cb9706004]
[fv-az99-305:14575] [ 9] plumed(+0xf698)[0x555cb9701698]
[fv-az99-305:14575] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f39169b10b3]
[fv-az99-305:14575] [11] plumed(+0xf76e)[0x555cb970176e]
[fv-az99-305:14575] *** End of error message ***
</pre>
{% endraw %}
