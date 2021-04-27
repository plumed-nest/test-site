**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_3-4/g2-w8-s4.697/plumed.dat   
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
[fv-az99-305:12437] *** Process received signal ***
[fv-az99-305:12437] Signal: Aborted (6)
[fv-az99-305:12437] Signal code:  (-6)
[fv-az99-305:12437] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fcc42496210]
[fv-az99-305:12437] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fcc4249618b]
[fv-az99-305:12437] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fcc42475859]
[fv-az99-305:12437] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fcc426fd951]
[fv-az99-305:12437] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fcc4270947c]
[fv-az99-305:12437] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fcc427094e7]
[fv-az99-305:12437] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fcc42709799]
[fv-az99-305:12437] [ 7] plumed(+0xf47d)[0x563380bbc47d]
[fv-az99-305:12437] [ 8] plumed(+0x14004)[0x563380bc1004]
[fv-az99-305:12437] [ 9] plumed(+0xf698)[0x563380bbc698]
[fv-az99-305:12437] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fcc424770b3]
[fv-az99-305:12437] [11] plumed(+0xf76e)[0x563380bbc76e]
[fv-az99-305:12437] *** End of error message ***
</pre>
{% endraw %}
