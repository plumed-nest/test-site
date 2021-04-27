**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_4-5prime/g1-w52-s9.711/plumed.dat   
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
[fv-az99-305:13935] *** Process received signal ***
[fv-az99-305:13935] Signal: Aborted (6)
[fv-az99-305:13935] Signal code:  (-6)
[fv-az99-305:13935] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7ffa8510d210]
[fv-az99-305:13935] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7ffa8510d18b]
[fv-az99-305:13935] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7ffa850ec859]
[fv-az99-305:13935] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7ffa85374951]
[fv-az99-305:13935] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7ffa8538047c]
[fv-az99-305:13935] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7ffa853804e7]
[fv-az99-305:13935] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7ffa85380799]
[fv-az99-305:13935] [ 7] plumed(+0xf47d)[0x561e3063c47d]
[fv-az99-305:13935] [ 8] plumed(+0x14004)[0x561e30641004]
[fv-az99-305:13935] [ 9] plumed(+0xf698)[0x561e3063c698]
[fv-az99-305:13935] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7ffa850ee0b3]
[fv-az99-305:13935] [11] plumed(+0xf76e)[0x561e3063c76e]
[fv-az99-305:13935] *** End of error message ***
</pre>
{% endraw %}
