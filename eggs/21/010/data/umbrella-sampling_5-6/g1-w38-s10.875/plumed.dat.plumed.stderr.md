**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_5-6/g1-w38-s10.875/plumed.dat   
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
[fv-az99-305:15136] *** Process received signal ***
[fv-az99-305:15136] Signal: Aborted (6)
[fv-az99-305:15136] Signal code:  (-6)
[fv-az99-305:15136] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fd9123bf210]
[fv-az99-305:15136] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fd9123bf18b]
[fv-az99-305:15136] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fd91239e859]
[fv-az99-305:15136] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fd912626951]
[fv-az99-305:15136] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fd91263247c]
[fv-az99-305:15136] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fd9126324e7]
[fv-az99-305:15136] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fd912632799]
[fv-az99-305:15136] [ 7] plumed(+0xf47d)[0x55e331c1b47d]
[fv-az99-305:15136] [ 8] plumed(+0x14004)[0x55e331c20004]
[fv-az99-305:15136] [ 9] plumed(+0xf698)[0x55e331c1b698]
[fv-az99-305:15136] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fd9123a00b3]
[fv-az99-305:15136] [11] plumed(+0xf76e)[0x55e331c1b76e]
[fv-az99-305:15136] *** End of error message ***
</pre>
{% endraw %}
