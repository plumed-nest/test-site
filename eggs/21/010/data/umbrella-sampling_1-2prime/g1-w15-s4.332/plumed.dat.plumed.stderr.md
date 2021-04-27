**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w15-s4.332/plumed.dat   
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
[fv-az99-305:08686] *** Process received signal ***
[fv-az99-305:08686] Signal: Aborted (6)
[fv-az99-305:08686] Signal code:  (-6)
[fv-az99-305:08686] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7faae9eae210]
[fv-az99-305:08686] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7faae9eae18b]
[fv-az99-305:08686] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7faae9e8d859]
[fv-az99-305:08686] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7faaea115951]
[fv-az99-305:08686] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7faaea12147c]
[fv-az99-305:08686] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7faaea1214e7]
[fv-az99-305:08686] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7faaea121799]
[fv-az99-305:08686] [ 7] plumed(+0xf47d)[0x557bb9fd247d]
[fv-az99-305:08686] [ 8] plumed(+0x14004)[0x557bb9fd7004]
[fv-az99-305:08686] [ 9] plumed(+0xf698)[0x557bb9fd2698]
[fv-az99-305:08686] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7faae9e8f0b3]
[fv-az99-305:08686] [11] plumed(+0xf76e)[0x557bb9fd276e]
[fv-az99-305:08686] *** End of error message ***
</pre>
{% endraw %}
