**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_4-5prime/g1-w51-s9.559/plumed.dat   
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
[fv-az99-305:13911] *** Process received signal ***
[fv-az99-305:13911] Signal: Aborted (6)
[fv-az99-305:13911] Signal code:  (-6)
[fv-az99-305:13911] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fbec8e70210]
[fv-az99-305:13911] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fbec8e7018b]
[fv-az99-305:13911] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fbec8e4f859]
[fv-az99-305:13911] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fbec90d7951]
[fv-az99-305:13911] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fbec90e347c]
[fv-az99-305:13911] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fbec90e34e7]
[fv-az99-305:13911] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fbec90e3799]
[fv-az99-305:13911] [ 7] plumed(+0xf47d)[0x55b8a87d647d]
[fv-az99-305:13911] [ 8] plumed(+0x14004)[0x55b8a87db004]
[fv-az99-305:13911] [ 9] plumed(+0xf698)[0x55b8a87d6698]
[fv-az99-305:13911] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fbec8e510b3]
[fv-az99-305:13911] [11] plumed(+0xf76e)[0x55b8a87d676e]
[fv-az99-305:13911] *** End of error message ***
</pre>
{% endraw %}
