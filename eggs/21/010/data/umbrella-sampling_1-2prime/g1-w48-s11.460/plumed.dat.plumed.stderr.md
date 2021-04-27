**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w48-s11.460/plumed.dat   
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
[fv-az99-305:09571] *** Process received signal ***
[fv-az99-305:09571] Signal: Aborted (6)
[fv-az99-305:09571] Signal code:  (-6)
[fv-az99-305:09571] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fc7d4fe2210]
[fv-az99-305:09571] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fc7d4fe218b]
[fv-az99-305:09571] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fc7d4fc1859]
[fv-az99-305:09571] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fc7d5249951]
[fv-az99-305:09571] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fc7d525547c]
[fv-az99-305:09571] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fc7d52554e7]
[fv-az99-305:09571] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fc7d5255799]
[fv-az99-305:09571] [ 7] plumed(+0xf47d)[0x55ef09c5d47d]
[fv-az99-305:09571] [ 8] plumed(+0x14004)[0x55ef09c62004]
[fv-az99-305:09571] [ 9] plumed(+0xf698)[0x55ef09c5d698]
[fv-az99-305:09571] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fc7d4fc30b3]
[fv-az99-305:09571] [11] plumed(+0xf76e)[0x55ef09c5d76e]
[fv-az99-305:09571] *** End of error message ***
</pre>
{% endraw %}
