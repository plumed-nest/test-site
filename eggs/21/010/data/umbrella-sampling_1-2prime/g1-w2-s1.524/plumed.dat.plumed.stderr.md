**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w2-s1.524/plumed.dat   
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
[fv-az99-305:08812] *** Process received signal ***
[fv-az99-305:08812] Signal: Aborted (6)
[fv-az99-305:08812] Signal code:  (-6)
[fv-az99-305:08812] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f255bb66210]
[fv-az99-305:08812] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f255bb6618b]
[fv-az99-305:08812] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f255bb45859]
[fv-az99-305:08812] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f255bdcd951]
[fv-az99-305:08812] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f255bdd947c]
[fv-az99-305:08812] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f255bdd94e7]
[fv-az99-305:08812] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f255bdd9799]
[fv-az99-305:08812] [ 7] plumed(+0xf47d)[0x56481484847d]
[fv-az99-305:08812] [ 8] plumed(+0x14004)[0x56481484d004]
[fv-az99-305:08812] [ 9] plumed(+0xf698)[0x564814848698]
[fv-az99-305:08812] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f255bb470b3]
[fv-az99-305:08812] [11] plumed(+0xf76e)[0x56481484876e]
[fv-az99-305:08812] *** End of error message ***
</pre>
{% endraw %}
