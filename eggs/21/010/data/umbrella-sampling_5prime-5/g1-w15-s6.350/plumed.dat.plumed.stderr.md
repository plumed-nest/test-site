**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_5prime-5/g1-w15-s6.350/plumed.dat   
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
[fv-az99-305:15752] *** Process received signal ***
[fv-az99-305:15752] Signal: Aborted (6)
[fv-az99-305:15752] Signal code:  (-6)
[fv-az99-305:15752] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fc568088210]
[fv-az99-305:15752] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fc56808818b]
[fv-az99-305:15752] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fc568067859]
[fv-az99-305:15752] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fc5682ef951]
[fv-az99-305:15752] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fc5682fb47c]
[fv-az99-305:15752] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fc5682fb4e7]
[fv-az99-305:15752] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fc5682fb799]
[fv-az99-305:15752] [ 7] plumed(+0xf47d)[0x557b9b3ad47d]
[fv-az99-305:15752] [ 8] plumed(+0x14004)[0x557b9b3b2004]
[fv-az99-305:15752] [ 9] plumed(+0xf698)[0x557b9b3ad698]
[fv-az99-305:15752] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fc5680690b3]
[fv-az99-305:15752] [11] plumed(+0xf76e)[0x557b9b3ad76e]
[fv-az99-305:15752] *** End of error message ***
</pre>
{% endraw %}
