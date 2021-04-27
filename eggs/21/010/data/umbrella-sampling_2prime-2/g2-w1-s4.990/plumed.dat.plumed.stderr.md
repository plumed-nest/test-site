**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_2prime-2/g2-w1-s4.990/plumed.dat   
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
[fv-az99-305:11407] *** Process received signal ***
[fv-az99-305:11407] Signal: Aborted (6)
[fv-az99-305:11407] Signal code:  (-6)
[fv-az99-305:11407] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fcec53e4210]
[fv-az99-305:11407] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fcec53e418b]
[fv-az99-305:11407] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fcec53c3859]
[fv-az99-305:11407] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fcec564b951]
[fv-az99-305:11407] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fcec565747c]
[fv-az99-305:11407] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fcec56574e7]
[fv-az99-305:11407] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fcec5657799]
[fv-az99-305:11407] [ 7] plumed(+0xf47d)[0x55f23113547d]
[fv-az99-305:11407] [ 8] plumed(+0x14004)[0x55f23113a004]
[fv-az99-305:11407] [ 9] plumed(+0xf698)[0x55f231135698]
[fv-az99-305:11407] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fcec53c50b3]
[fv-az99-305:11407] [11] plumed(+0xf76e)[0x55f23113576e]
[fv-az99-305:11407] *** End of error message ***
</pre>
{% endraw %}
