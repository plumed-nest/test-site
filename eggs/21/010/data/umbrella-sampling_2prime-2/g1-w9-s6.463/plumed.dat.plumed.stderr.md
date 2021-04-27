**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_2prime-2/g1-w9-s6.463/plumed.dat   
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
[fv-az99-305:11383] *** Process received signal ***
[fv-az99-305:11383] Signal: Aborted (6)
[fv-az99-305:11383] Signal code:  (-6)
[fv-az99-305:11383] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f7b5a677210]
[fv-az99-305:11383] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f7b5a67718b]
[fv-az99-305:11383] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f7b5a656859]
[fv-az99-305:11383] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f7b5a8de951]
[fv-az99-305:11383] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f7b5a8ea47c]
[fv-az99-305:11383] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f7b5a8ea4e7]
[fv-az99-305:11383] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f7b5a8ea799]
[fv-az99-305:11383] [ 7] plumed(+0xf47d)[0x562967f3c47d]
[fv-az99-305:11383] [ 8] plumed(+0x14004)[0x562967f41004]
[fv-az99-305:11383] [ 9] plumed(+0xf698)[0x562967f3c698]
[fv-az99-305:11383] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f7b5a6580b3]
[fv-az99-305:11383] [11] plumed(+0xf76e)[0x562967f3c76e]
[fv-az99-305:11383] *** End of error message ***
</pre>
{% endraw %}
