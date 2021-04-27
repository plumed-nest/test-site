**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_3-4/g2-w16-s6.774/plumed.dat   
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
[fv-az99-305:12022] *** Process received signal ***
[fv-az99-305:12022] Signal: Aborted (6)
[fv-az99-305:12022] Signal code:  (-6)
[fv-az99-305:12022] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f20b3cf6210]
[fv-az99-305:12022] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f20b3cf618b]
[fv-az99-305:12022] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f20b3cd5859]
[fv-az99-305:12022] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f20b3f5d951]
[fv-az99-305:12022] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f20b3f6947c]
[fv-az99-305:12022] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f20b3f694e7]
[fv-az99-305:12022] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f20b3f69799]
[fv-az99-305:12022] [ 7] plumed(+0xf47d)[0x560c0bf6147d]
[fv-az99-305:12022] [ 8] plumed(+0x14004)[0x560c0bf66004]
[fv-az99-305:12022] [ 9] plumed(+0xf698)[0x560c0bf61698]
[fv-az99-305:12022] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f20b3cd70b3]
[fv-az99-305:12022] [11] plumed(+0xf76e)[0x560c0bf6176e]
[fv-az99-305:12022] *** End of error message ***
</pre>
{% endraw %}
