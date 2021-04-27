**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_4-5prime/g1-w7-s2.886/plumed.dat   
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
[fv-az99-305:14179] *** Process received signal ***
[fv-az99-305:14179] Signal: Aborted (6)
[fv-az99-305:14179] Signal code:  (-6)
[fv-az99-305:14179] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fb14203c210]
[fv-az99-305:14179] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fb14203c18b]
[fv-az99-305:14179] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fb14201b859]
[fv-az99-305:14179] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fb1422a3951]
[fv-az99-305:14179] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fb1422af47c]
[fv-az99-305:14179] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fb1422af4e7]
[fv-az99-305:14179] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fb1422af799]
[fv-az99-305:14179] [ 7] plumed(+0xf47d)[0x55788b26247d]
[fv-az99-305:14179] [ 8] plumed(+0x14004)[0x55788b267004]
[fv-az99-305:14179] [ 9] plumed(+0xf698)[0x55788b262698]
[fv-az99-305:14179] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fb14201d0b3]
[fv-az99-305:14179] [11] plumed(+0xf76e)[0x55788b26276e]
[fv-az99-305:14179] *** End of error message ***
</pre>
{% endraw %}
