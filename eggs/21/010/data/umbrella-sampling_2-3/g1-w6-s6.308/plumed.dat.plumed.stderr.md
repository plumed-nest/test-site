**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_2-3/g1-w6-s6.308/plumed.dat   
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
[fv-az99-305:10530] *** Process received signal ***
[fv-az99-305:10530] Signal: Aborted (6)
[fv-az99-305:10530] Signal code:  (-6)
[fv-az99-305:10530] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f95b1ef0210]
[fv-az99-305:10530] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f95b1ef018b]
[fv-az99-305:10530] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f95b1ecf859]
[fv-az99-305:10530] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f95b2157951]
[fv-az99-305:10530] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f95b216347c]
[fv-az99-305:10530] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f95b21634e7]
[fv-az99-305:10530] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f95b2163799]
[fv-az99-305:10530] [ 7] plumed(+0xf47d)[0x55ac5fa1a47d]
[fv-az99-305:10530] [ 8] plumed(+0x14004)[0x55ac5fa1f004]
[fv-az99-305:10530] [ 9] plumed(+0xf698)[0x55ac5fa1a698]
[fv-az99-305:10530] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f95b1ed10b3]
[fv-az99-305:10530] [11] plumed(+0xf76e)[0x55ac5fa1a76e]
[fv-az99-305:10530] *** End of error message ***
</pre>
{% endraw %}
