**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_4-5prime/g1-w40-s7.891/plumed.dat   
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
[fv-az99-305:13618] *** Process received signal ***
[fv-az99-305:13618] Signal: Aborted (6)
[fv-az99-305:13618] Signal code:  (-6)
[fv-az99-305:13618] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f94f863d210]
[fv-az99-305:13618] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f94f863d18b]
[fv-az99-305:13618] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f94f861c859]
[fv-az99-305:13618] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f94f88a4951]
[fv-az99-305:13618] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f94f88b047c]
[fv-az99-305:13618] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f94f88b04e7]
[fv-az99-305:13618] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f94f88b0799]
[fv-az99-305:13618] [ 7] plumed(+0xf47d)[0x55d48b33a47d]
[fv-az99-305:13618] [ 8] plumed(+0x14004)[0x55d48b33f004]
[fv-az99-305:13618] [ 9] plumed(+0xf698)[0x55d48b33a698]
[fv-az99-305:13618] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f94f861e0b3]
[fv-az99-305:13618] [11] plumed(+0xf76e)[0x55d48b33a76e]
[fv-az99-305:13618] *** End of error message ***
</pre>
{% endraw %}
