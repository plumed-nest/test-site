**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_2prime-2/g1-w7-s6.213/plumed.dat   
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
[fv-az99-305:11333] *** Process received signal ***
[fv-az99-305:11333] Signal: Aborted (6)
[fv-az99-305:11333] Signal code:  (-6)
[fv-az99-305:11333] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f7339aac210]
[fv-az99-305:11333] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f7339aac18b]
[fv-az99-305:11333] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f7339a8b859]
[fv-az99-305:11333] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f7339d13951]
[fv-az99-305:11333] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f7339d1f47c]
[fv-az99-305:11333] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f7339d1f4e7]
[fv-az99-305:11333] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f7339d1f799]
[fv-az99-305:11333] [ 7] plumed(+0xf47d)[0x55bf3832e47d]
[fv-az99-305:11333] [ 8] plumed(+0x14004)[0x55bf38333004]
[fv-az99-305:11333] [ 9] plumed(+0xf698)[0x55bf3832e698]
[fv-az99-305:11333] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f7339a8d0b3]
[fv-az99-305:11333] [11] plumed(+0xf76e)[0x55bf3832e76e]
[fv-az99-305:11333] *** End of error message ***
</pre>
{% endraw %}
