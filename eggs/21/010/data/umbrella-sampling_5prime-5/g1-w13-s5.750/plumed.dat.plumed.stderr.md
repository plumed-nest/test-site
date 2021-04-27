**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_5prime-5/g1-w13-s5.750/plumed.dat   
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
[fv-az99-305:15701] *** Process received signal ***
[fv-az99-305:15701] Signal: Aborted (6)
[fv-az99-305:15701] Signal code:  (-6)
[fv-az99-305:15701] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fee32c70210]
[fv-az99-305:15701] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fee32c7018b]
[fv-az99-305:15701] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fee32c4f859]
[fv-az99-305:15701] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fee32ed7951]
[fv-az99-305:15701] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fee32ee347c]
[fv-az99-305:15701] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fee32ee34e7]
[fv-az99-305:15701] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fee32ee3799]
[fv-az99-305:15701] [ 7] plumed(+0xf47d)[0x555d9abd247d]
[fv-az99-305:15701] [ 8] plumed(+0x14004)[0x555d9abd7004]
[fv-az99-305:15701] [ 9] plumed(+0xf698)[0x555d9abd2698]
[fv-az99-305:15701] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fee32c510b3]
[fv-az99-305:15701] [11] plumed(+0xf76e)[0x555d9abd276e]
[fv-az99-305:15701] *** End of error message ***
</pre>
{% endraw %}
