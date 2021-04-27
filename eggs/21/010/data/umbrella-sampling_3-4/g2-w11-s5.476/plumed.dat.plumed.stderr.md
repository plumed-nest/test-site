**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_3-4/g2-w11-s5.476/plumed.dat   
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
[fv-az99-305:11897] *** Process received signal ***
[fv-az99-305:11897] Signal: Aborted (6)
[fv-az99-305:11897] Signal code:  (-6)
[fv-az99-305:11897] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f2716b74210]
[fv-az99-305:11897] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f2716b7418b]
[fv-az99-305:11897] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f2716b53859]
[fv-az99-305:11897] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f2716ddb951]
[fv-az99-305:11897] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f2716de747c]
[fv-az99-305:11897] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f2716de74e7]
[fv-az99-305:11897] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f2716de7799]
[fv-az99-305:11897] [ 7] plumed(+0xf47d)[0x557f9729047d]
[fv-az99-305:11897] [ 8] plumed(+0x14004)[0x557f97295004]
[fv-az99-305:11897] [ 9] plumed(+0xf698)[0x557f97290698]
[fv-az99-305:11897] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f2716b550b3]
[fv-az99-305:11897] [11] plumed(+0xf76e)[0x557f9729076e]
[fv-az99-305:11897] *** End of error message ***
</pre>
{% endraw %}
