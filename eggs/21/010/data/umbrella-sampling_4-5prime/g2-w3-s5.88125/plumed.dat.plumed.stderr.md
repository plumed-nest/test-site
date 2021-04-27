**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_4-5prime/g2-w3-s5.88125/plumed.dat   
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
[fv-az99-305:14304] *** Process received signal ***
[fv-az99-305:14304] Signal: Aborted (6)
[fv-az99-305:14304] Signal code:  (-6)
[fv-az99-305:14304] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fbc2e3a2210]
[fv-az99-305:14304] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fbc2e3a218b]
[fv-az99-305:14304] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fbc2e381859]
[fv-az99-305:14304] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fbc2e609951]
[fv-az99-305:14304] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fbc2e61547c]
[fv-az99-305:14304] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fbc2e6154e7]
[fv-az99-305:14304] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fbc2e615799]
[fv-az99-305:14304] [ 7] plumed(+0xf47d)[0x557e62d7947d]
[fv-az99-305:14304] [ 8] plumed(+0x14004)[0x557e62d7e004]
[fv-az99-305:14304] [ 9] plumed(+0xf698)[0x557e62d79698]
[fv-az99-305:14304] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fbc2e3830b3]
[fv-az99-305:14304] [11] plumed(+0xf76e)[0x557e62d7976e]
[fv-az99-305:14304] *** End of error message ***
</pre>
{% endraw %}
