**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w8-s2.820/plumed.dat   
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
[fv-az99-305:09722] *** Process received signal ***
[fv-az99-305:09722] Signal: Aborted (6)
[fv-az99-305:09722] Signal code:  (-6)
[fv-az99-305:09722] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fb8df5c1210]
[fv-az99-305:09722] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fb8df5c118b]
[fv-az99-305:09722] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fb8df5a0859]
[fv-az99-305:09722] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fb8df828951]
[fv-az99-305:09722] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fb8df83447c]
[fv-az99-305:09722] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fb8df8344e7]
[fv-az99-305:09722] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fb8df834799]
[fv-az99-305:09722] [ 7] plumed(+0xf47d)[0x561b0d1cf47d]
[fv-az99-305:09722] [ 8] plumed(+0x14004)[0x561b0d1d4004]
[fv-az99-305:09722] [ 9] plumed(+0xf698)[0x561b0d1cf698]
[fv-az99-305:09722] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fb8df5a20b3]
[fv-az99-305:09722] [11] plumed(+0xf76e)[0x561b0d1cf76e]
[fv-az99-305:09722] *** End of error message ***
</pre>
{% endraw %}
