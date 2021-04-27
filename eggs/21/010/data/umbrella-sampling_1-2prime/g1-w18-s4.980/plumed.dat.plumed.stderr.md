**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w18-s4.980/plumed.dat   
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
[fv-az99-305:08759] *** Process received signal ***
[fv-az99-305:08759] Signal: Aborted (6)
[fv-az99-305:08759] Signal code:  (-6)
[fv-az99-305:08759] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f80672f8210]
[fv-az99-305:08759] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f80672f818b]
[fv-az99-305:08759] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f80672d7859]
[fv-az99-305:08759] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f806755f951]
[fv-az99-305:08759] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f806756b47c]
[fv-az99-305:08759] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f806756b4e7]
[fv-az99-305:08759] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f806756b799]
[fv-az99-305:08759] [ 7] plumed(+0xf47d)[0x5649c0f4c47d]
[fv-az99-305:08759] [ 8] plumed(+0x14004)[0x5649c0f51004]
[fv-az99-305:08759] [ 9] plumed(+0xf698)[0x5649c0f4c698]
[fv-az99-305:08759] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f80672d90b3]
[fv-az99-305:08759] [11] plumed(+0xf76e)[0x5649c0f4c76e]
[fv-az99-305:08759] *** End of error message ***
</pre>
{% endraw %}
