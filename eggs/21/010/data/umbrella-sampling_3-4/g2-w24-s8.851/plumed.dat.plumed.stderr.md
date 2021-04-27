**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_3-4/g2-w24-s8.851/plumed.dat   
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
[fv-az99-305:12240] *** Process received signal ***
[fv-az99-305:12240] Signal: Aborted (6)
[fv-az99-305:12240] Signal code:  (-6)
[fv-az99-305:12240] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fe838408210]
[fv-az99-305:12240] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fe83840818b]
[fv-az99-305:12240] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fe8383e7859]
[fv-az99-305:12240] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fe83866f951]
[fv-az99-305:12240] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fe83867b47c]
[fv-az99-305:12240] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fe83867b4e7]
[fv-az99-305:12240] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fe83867b799]
[fv-az99-305:12240] [ 7] plumed(+0xf47d)[0x55aa9cc9247d]
[fv-az99-305:12240] [ 8] plumed(+0x14004)[0x55aa9cc97004]
[fv-az99-305:12240] [ 9] plumed(+0xf698)[0x55aa9cc92698]
[fv-az99-305:12240] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fe8383e90b3]
[fv-az99-305:12240] [11] plumed(+0xf76e)[0x55aa9cc9276e]
[fv-az99-305:12240] *** End of error message ***
</pre>
{% endraw %}
