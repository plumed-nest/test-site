**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_4-5prime/g1-w19-s4.706/plumed.dat   
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
[fv-az99-305:13030] *** Process received signal ***
[fv-az99-305:13030] Signal: Aborted (6)
[fv-az99-305:13030] Signal code:  (-6)
[fv-az99-305:13030] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fc8e76c0210]
[fv-az99-305:13030] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fc8e76c018b]
[fv-az99-305:13030] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fc8e769f859]
[fv-az99-305:13030] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fc8e7927951]
[fv-az99-305:13030] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fc8e793347c]
[fv-az99-305:13030] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fc8e79334e7]
[fv-az99-305:13030] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fc8e7933799]
[fv-az99-305:13030] [ 7] plumed(+0xf47d)[0x559dc732b47d]
[fv-az99-305:13030] [ 8] plumed(+0x14004)[0x559dc7330004]
[fv-az99-305:13030] [ 9] plumed(+0xf698)[0x559dc732b698]
[fv-az99-305:13030] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fc8e76a10b3]
[fv-az99-305:13030] [11] plumed(+0xf76e)[0x559dc732b76e]
[fv-az99-305:13030] *** End of error message ***
</pre>
{% endraw %}
