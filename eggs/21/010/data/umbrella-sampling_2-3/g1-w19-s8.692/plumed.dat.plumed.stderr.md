**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_2-3/g1-w19-s8.692/plumed.dat   
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
[fv-az99-305:10188] *** Process received signal ***
[fv-az99-305:10188] Signal: Aborted (6)
[fv-az99-305:10188] Signal code:  (-6)
[fv-az99-305:10188] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f7e6e23e210]
[fv-az99-305:10188] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f7e6e23e18b]
[fv-az99-305:10188] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f7e6e21d859]
[fv-az99-305:10188] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f7e6e4a5951]
[fv-az99-305:10188] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f7e6e4b147c]
[fv-az99-305:10188] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f7e6e4b14e7]
[fv-az99-305:10188] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f7e6e4b1799]
[fv-az99-305:10188] [ 7] plumed(+0xf47d)[0x5590603ee47d]
[fv-az99-305:10188] [ 8] plumed(+0x14004)[0x5590603f3004]
[fv-az99-305:10188] [ 9] plumed(+0xf698)[0x5590603ee698]
[fv-az99-305:10188] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f7e6e21f0b3]
[fv-az99-305:10188] [11] plumed(+0xf76e)[0x5590603ee76e]
[fv-az99-305:10188] *** End of error message ***
</pre>
{% endraw %}
