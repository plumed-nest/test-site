**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_2-3/g2-w3-s5.257/plumed.dat   
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
[fv-az99-305:10770] *** Process received signal ***
[fv-az99-305:10770] Signal: Aborted (6)
[fv-az99-305:10770] Signal code:  (-6)
[fv-az99-305:10770] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f13166d2210]
[fv-az99-305:10770] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f13166d218b]
[fv-az99-305:10770] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f13166b1859]
[fv-az99-305:10770] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f1316939951]
[fv-az99-305:10770] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f131694547c]
[fv-az99-305:10770] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f13169454e7]
[fv-az99-305:10770] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f1316945799]
[fv-az99-305:10770] [ 7] plumed(+0xf47d)[0x56373d7c447d]
[fv-az99-305:10770] [ 8] plumed(+0x14004)[0x56373d7c9004]
[fv-az99-305:10770] [ 9] plumed(+0xf698)[0x56373d7c4698]
[fv-az99-305:10770] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f13166b30b3]
[fv-az99-305:10770] [11] plumed(+0xf76e)[0x56373d7c476e]
[fv-az99-305:10770] *** End of error message ***
</pre>
{% endraw %}
