**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w11-s3.468/plumed.dat   
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
[fv-az99-305:08589] *** Process received signal ***
[fv-az99-305:08589] Signal: Aborted (6)
[fv-az99-305:08589] Signal code:  (-6)
[fv-az99-305:08589] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fb52f3b4210]
[fv-az99-305:08589] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fb52f3b418b]
[fv-az99-305:08589] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fb52f393859]
[fv-az99-305:08589] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fb52f61b951]
[fv-az99-305:08589] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fb52f62747c]
[fv-az99-305:08589] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fb52f6274e7]
[fv-az99-305:08589] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fb52f627799]
[fv-az99-305:08589] [ 7] plumed(+0xf47d)[0x56068384647d]
[fv-az99-305:08589] [ 8] plumed(+0x14004)[0x56068384b004]
[fv-az99-305:08589] [ 9] plumed(+0xf698)[0x560683846698]
[fv-az99-305:08589] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fb52f3950b3]
[fv-az99-305:08589] [11] plumed(+0xf76e)[0x56068384676e]
[fv-az99-305:08589] *** End of error message ***
</pre>
{% endraw %}
