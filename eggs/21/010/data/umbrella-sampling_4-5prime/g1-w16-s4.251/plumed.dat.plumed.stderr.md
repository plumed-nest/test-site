**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_4-5prime/g1-w16-s4.251/plumed.dat   
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
[fv-az99-305:12957] *** Process received signal ***
[fv-az99-305:12957] Signal: Aborted (6)
[fv-az99-305:12957] Signal code:  (-6)
[fv-az99-305:12957] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f9d5c351210]
[fv-az99-305:12957] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f9d5c35118b]
[fv-az99-305:12957] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f9d5c330859]
[fv-az99-305:12957] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f9d5c5b8951]
[fv-az99-305:12957] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f9d5c5c447c]
[fv-az99-305:12957] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f9d5c5c44e7]
[fv-az99-305:12957] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f9d5c5c4799]
[fv-az99-305:12957] [ 7] plumed(+0xf47d)[0x557c24cec47d]
[fv-az99-305:12957] [ 8] plumed(+0x14004)[0x557c24cf1004]
[fv-az99-305:12957] [ 9] plumed(+0xf698)[0x557c24cec698]
[fv-az99-305:12957] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f9d5c3320b3]
[fv-az99-305:12957] [11] plumed(+0xf76e)[0x557c24cec76e]
[fv-az99-305:12957] *** End of error message ***
</pre>
{% endraw %}
