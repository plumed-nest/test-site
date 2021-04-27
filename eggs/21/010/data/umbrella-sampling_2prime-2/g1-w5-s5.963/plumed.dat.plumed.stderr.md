**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_2prime-2/g1-w5-s5.963/plumed.dat   
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
[fv-az99-305:11284] *** Process received signal ***
[fv-az99-305:11284] Signal: Aborted (6)
[fv-az99-305:11284] Signal code:  (-6)
[fv-az99-305:11284] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f7ac7d98210]
[fv-az99-305:11284] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f7ac7d9818b]
[fv-az99-305:11284] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f7ac7d77859]
[fv-az99-305:11284] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f7ac7fff951]
[fv-az99-305:11284] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f7ac800b47c]
[fv-az99-305:11284] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f7ac800b4e7]
[fv-az99-305:11284] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f7ac800b799]
[fv-az99-305:11284] [ 7] plumed(+0xf47d)[0x5654a30cb47d]
[fv-az99-305:11284] [ 8] plumed(+0x14004)[0x5654a30d0004]
[fv-az99-305:11284] [ 9] plumed(+0xf698)[0x5654a30cb698]
[fv-az99-305:11284] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f7ac7d790b3]
[fv-az99-305:11284] [11] plumed(+0xf76e)[0x5654a30cb76e]
[fv-az99-305:11284] *** End of error message ***
</pre>
{% endraw %}
