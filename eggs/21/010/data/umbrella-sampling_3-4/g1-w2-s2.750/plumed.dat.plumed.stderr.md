**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_3-4/g1-w2-s2.750/plumed.dat   
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
[fv-az99-305:11825] *** Process received signal ***
[fv-az99-305:11825] Signal: Aborted (6)
[fv-az99-305:11825] Signal code:  (-6)
[fv-az99-305:11825] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f774860e210]
[fv-az99-305:11825] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f774860e18b]
[fv-az99-305:11825] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f77485ed859]
[fv-az99-305:11825] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f7748875951]
[fv-az99-305:11825] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f774888147c]
[fv-az99-305:11825] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f77488814e7]
[fv-az99-305:11825] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f7748881799]
[fv-az99-305:11825] [ 7] plumed(+0xf47d)[0x556a0f41847d]
[fv-az99-305:11825] [ 8] plumed(+0x14004)[0x556a0f41d004]
[fv-az99-305:11825] [ 9] plumed(+0xf698)[0x556a0f418698]
[fv-az99-305:11825] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f77485ef0b3]
[fv-az99-305:11825] [11] plumed(+0xf76e)[0x556a0f41876e]
[fv-az99-305:11825] *** End of error message ***
</pre>
{% endraw %}
