**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_2prime-2/g1-w23-s8.213/plumed.dat   
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
[fv-az99-305:11187] *** Process received signal ***
[fv-az99-305:11187] Signal: Aborted (6)
[fv-az99-305:11187] Signal code:  (-6)
[fv-az99-305:11187] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fdd2d3ee210]
[fv-az99-305:11187] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fdd2d3ee18b]
[fv-az99-305:11187] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fdd2d3cd859]
[fv-az99-305:11187] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fdd2d655951]
[fv-az99-305:11187] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fdd2d66147c]
[fv-az99-305:11187] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fdd2d6614e7]
[fv-az99-305:11187] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fdd2d661799]
[fv-az99-305:11187] [ 7] plumed(+0xf47d)[0x55650e71a47d]
[fv-az99-305:11187] [ 8] plumed(+0x14004)[0x55650e71f004]
[fv-az99-305:11187] [ 9] plumed(+0xf698)[0x55650e71a698]
[fv-az99-305:11187] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fdd2d3cf0b3]
[fv-az99-305:11187] [11] plumed(+0xf76e)[0x55650e71a76e]
[fv-az99-305:11187] *** End of error message ***
</pre>
{% endraw %}
