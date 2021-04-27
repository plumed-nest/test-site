**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_2prime-2/g2-w2-s8.709/plumed.dat   
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
[fv-az99-305:11480] *** Process received signal ***
[fv-az99-305:11480] Signal: Aborted (6)
[fv-az99-305:11480] Signal code:  (-6)
[fv-az99-305:11480] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f955f0bc210]
[fv-az99-305:11480] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f955f0bc18b]
[fv-az99-305:11480] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f955f09b859]
[fv-az99-305:11480] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f955f323951]
[fv-az99-305:11480] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f955f32f47c]
[fv-az99-305:11480] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f955f32f4e7]
[fv-az99-305:11480] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f955f32f799]
[fv-az99-305:11480] [ 7] plumed(+0xf47d)[0x55bd244db47d]
[fv-az99-305:11480] [ 8] plumed(+0x14004)[0x55bd244e0004]
[fv-az99-305:11480] [ 9] plumed(+0xf698)[0x55bd244db698]
[fv-az99-305:11480] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f955f09d0b3]
[fv-az99-305:11480] [11] plumed(+0xf76e)[0x55bd244db76e]
[fv-az99-305:11480] *** End of error message ***
</pre>
{% endraw %}
