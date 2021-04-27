**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_4-5prime/g1-w59-s10.773/plumed.dat   
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
[fv-az99-305:14107] *** Process received signal ***
[fv-az99-305:14107] Signal: Aborted (6)
[fv-az99-305:14107] Signal code:  (-6)
[fv-az99-305:14107] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fe406fff210]
[fv-az99-305:14107] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fe406fff18b]
[fv-az99-305:14107] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fe406fde859]
[fv-az99-305:14107] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fe407266951]
[fv-az99-305:14107] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fe40727247c]
[fv-az99-305:14107] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fe4072724e7]
[fv-az99-305:14107] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fe407272799]
[fv-az99-305:14107] [ 7] plumed(+0xf47d)[0x557af074047d]
[fv-az99-305:14107] [ 8] plumed(+0x14004)[0x557af0745004]
[fv-az99-305:14107] [ 9] plumed(+0xf698)[0x557af0740698]
[fv-az99-305:14107] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fe406fe00b3]
[fv-az99-305:14107] [11] plumed(+0xf76e)[0x557af074076e]
[fv-az99-305:14107] *** End of error message ***
</pre>
{% endraw %}
