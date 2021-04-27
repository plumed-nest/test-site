**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w13-s3.900/plumed.dat   
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
[fv-az99-305:08638] *** Process received signal ***
[fv-az99-305:08638] Signal: Aborted (6)
[fv-az99-305:08638] Signal code:  (-6)
[fv-az99-305:08638] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fe152e28210]
[fv-az99-305:08638] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fe152e2818b]
[fv-az99-305:08638] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fe152e07859]
[fv-az99-305:08638] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fe15308f951]
[fv-az99-305:08638] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fe15309b47c]
[fv-az99-305:08638] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fe15309b4e7]
[fv-az99-305:08638] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fe15309b799]
[fv-az99-305:08638] [ 7] plumed(+0xf47d)[0x55976bc5b47d]
[fv-az99-305:08638] [ 8] plumed(+0x14004)[0x55976bc60004]
[fv-az99-305:08638] [ 9] plumed(+0xf698)[0x55976bc5b698]
[fv-az99-305:08638] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fe152e090b3]
[fv-az99-305:08638] [11] plumed(+0xf76e)[0x55976bc5b76e]
[fv-az99-305:08638] *** End of error message ***
</pre>
{% endraw %}
