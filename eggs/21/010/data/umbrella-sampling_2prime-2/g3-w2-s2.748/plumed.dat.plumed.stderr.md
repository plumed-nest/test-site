**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_2prime-2/g3-w2-s2.748/plumed.dat   
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
[fv-az99-305:11529] *** Process received signal ***
[fv-az99-305:11529] Signal: Aborted (6)
[fv-az99-305:11529] Signal code:  (-6)
[fv-az99-305:11529] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f9136c89210]
[fv-az99-305:11529] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f9136c8918b]
[fv-az99-305:11529] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f9136c68859]
[fv-az99-305:11529] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f9136ef0951]
[fv-az99-305:11529] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f9136efc47c]
[fv-az99-305:11529] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f9136efc4e7]
[fv-az99-305:11529] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f9136efc799]
[fv-az99-305:11529] [ 7] plumed(+0xf47d)[0x5567188a647d]
[fv-az99-305:11529] [ 8] plumed(+0x14004)[0x5567188ab004]
[fv-az99-305:11529] [ 9] plumed(+0xf698)[0x5567188a6698]
[fv-az99-305:11529] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f9136c6a0b3]
[fv-az99-305:11529] [11] plumed(+0xf76e)[0x5567188a676e]
[fv-az99-305:11529] *** End of error message ***
</pre>
{% endraw %}
