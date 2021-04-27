**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_2prime-2/g1-w19-s7.713/plumed.dat   
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
[fv-az99-305:11063] *** Process received signal ***
[fv-az99-305:11063] Signal: Aborted (6)
[fv-az99-305:11063] Signal code:  (-6)
[fv-az99-305:11063] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f98b0c58210]
[fv-az99-305:11063] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f98b0c5818b]
[fv-az99-305:11063] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f98b0c37859]
[fv-az99-305:11063] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f98b0ebf951]
[fv-az99-305:11063] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f98b0ecb47c]
[fv-az99-305:11063] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f98b0ecb4e7]
[fv-az99-305:11063] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f98b0ecb799]
[fv-az99-305:11063] [ 7] plumed(+0xf47d)[0x55e0f939547d]
[fv-az99-305:11063] [ 8] plumed(+0x14004)[0x55e0f939a004]
[fv-az99-305:11063] [ 9] plumed(+0xf698)[0x55e0f9395698]
[fv-az99-305:11063] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f98b0c390b3]
[fv-az99-305:11063] [11] plumed(+0xf76e)[0x55e0f939576e]
[fv-az99-305:11063] *** End of error message ***
</pre>
{% endraw %}
