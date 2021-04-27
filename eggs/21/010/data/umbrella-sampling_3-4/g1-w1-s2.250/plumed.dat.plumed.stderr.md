**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_3-4/g1-w1-s2.250/plumed.dat   
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
[fv-az99-305:11800] *** Process received signal ***
[fv-az99-305:11800] Signal: Aborted (6)
[fv-az99-305:11800] Signal code:  (-6)
[fv-az99-305:11800] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f62b19d2210]
[fv-az99-305:11800] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f62b19d218b]
[fv-az99-305:11800] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f62b19b1859]
[fv-az99-305:11800] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f62b1c39951]
[fv-az99-305:11800] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f62b1c4547c]
[fv-az99-305:11800] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f62b1c454e7]
[fv-az99-305:11800] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f62b1c45799]
[fv-az99-305:11800] [ 7] plumed(+0xf47d)[0x557d8d5f747d]
[fv-az99-305:11800] [ 8] plumed(+0x14004)[0x557d8d5fc004]
[fv-az99-305:11800] [ 9] plumed(+0xf698)[0x557d8d5f7698]
[fv-az99-305:11800] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f62b19b30b3]
[fv-az99-305:11800] [11] plumed(+0xf76e)[0x557d8d5f776e]
[fv-az99-305:11800] *** End of error message ***
</pre>
{% endraw %}
