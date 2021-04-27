**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w17-s4.764/plumed.dat   
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
[fv-az99-305:08735] *** Process received signal ***
[fv-az99-305:08735] Signal: Aborted (6)
[fv-az99-305:08735] Signal code:  (-6)
[fv-az99-305:08735] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f5f8498c210]
[fv-az99-305:08735] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f5f8498c18b]
[fv-az99-305:08735] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f5f8496b859]
[fv-az99-305:08735] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f5f84bf3951]
[fv-az99-305:08735] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f5f84bff47c]
[fv-az99-305:08735] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f5f84bff4e7]
[fv-az99-305:08735] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f5f84bff799]
[fv-az99-305:08735] [ 7] plumed(+0xf47d)[0x55d68f4bc47d]
[fv-az99-305:08735] [ 8] plumed(+0x14004)[0x55d68f4c1004]
[fv-az99-305:08735] [ 9] plumed(+0xf698)[0x55d68f4bc698]
[fv-az99-305:08735] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f5f8496d0b3]
[fv-az99-305:08735] [11] plumed(+0xf76e)[0x55d68f4bc76e]
[fv-az99-305:08735] *** End of error message ***
</pre>
{% endraw %}
