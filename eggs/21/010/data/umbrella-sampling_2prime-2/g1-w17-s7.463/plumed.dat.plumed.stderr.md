**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_2prime-2/g1-w17-s7.463/plumed.dat   
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
[fv-az99-305:11014] *** Process received signal ***
[fv-az99-305:11014] Signal: Aborted (6)
[fv-az99-305:11014] Signal code:  (-6)
[fv-az99-305:11014] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7efff491c210]
[fv-az99-305:11014] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7efff491c18b]
[fv-az99-305:11014] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7efff48fb859]
[fv-az99-305:11014] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7efff4b83951]
[fv-az99-305:11014] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7efff4b8f47c]
[fv-az99-305:11014] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7efff4b8f4e7]
[fv-az99-305:11014] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7efff4b8f799]
[fv-az99-305:11014] [ 7] plumed(+0xf47d)[0x560b14b4e47d]
[fv-az99-305:11014] [ 8] plumed(+0x14004)[0x560b14b53004]
[fv-az99-305:11014] [ 9] plumed(+0xf698)[0x560b14b4e698]
[fv-az99-305:11014] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7efff48fd0b3]
[fv-az99-305:11014] [11] plumed(+0xf76e)[0x560b14b4e76e]
[fv-az99-305:11014] *** End of error message ***
</pre>
{% endraw %}
