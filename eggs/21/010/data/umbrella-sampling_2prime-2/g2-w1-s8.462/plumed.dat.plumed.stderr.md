**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_2prime-2/g2-w1-s8.462/plumed.dat   
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
[fv-az99-305:11432] *** Process received signal ***
[fv-az99-305:11432] Signal: Aborted (6)
[fv-az99-305:11432] Signal code:  (-6)
[fv-az99-305:11432] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fe2cfde2210]
[fv-az99-305:11432] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fe2cfde218b]
[fv-az99-305:11432] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fe2cfdc1859]
[fv-az99-305:11432] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fe2d0049951]
[fv-az99-305:11432] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fe2d005547c]
[fv-az99-305:11432] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fe2d00554e7]
[fv-az99-305:11432] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fe2d0055799]
[fv-az99-305:11432] [ 7] plumed(+0xf47d)[0x55be0cce147d]
[fv-az99-305:11432] [ 8] plumed(+0x14004)[0x55be0cce6004]
[fv-az99-305:11432] [ 9] plumed(+0xf698)[0x55be0cce1698]
[fv-az99-305:11432] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fe2cfdc30b3]
[fv-az99-305:11432] [11] plumed(+0xf76e)[0x55be0cce176e]
[fv-az99-305:11432] *** End of error message ***
</pre>
{% endraw %}
