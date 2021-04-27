**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_2-3/g1-w11-s7.225/plumed.dat   
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
[fv-az99-305:09993] *** Process received signal ***
[fv-az99-305:09993] Signal: Aborted (6)
[fv-az99-305:09993] Signal code:  (-6)
[fv-az99-305:09993] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f0456d61210]
[fv-az99-305:09993] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f0456d6118b]
[fv-az99-305:09993] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f0456d40859]
[fv-az99-305:09993] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f0456fc8951]
[fv-az99-305:09993] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f0456fd447c]
[fv-az99-305:09993] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f0456fd44e7]
[fv-az99-305:09993] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f0456fd4799]
[fv-az99-305:09993] [ 7] plumed(+0xf47d)[0x562f96b8847d]
[fv-az99-305:09993] [ 8] plumed(+0x14004)[0x562f96b8d004]
[fv-az99-305:09993] [ 9] plumed(+0xf698)[0x562f96b88698]
[fv-az99-305:09993] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f0456d420b3]
[fv-az99-305:09993] [11] plumed(+0xf76e)[0x562f96b8876e]
[fv-az99-305:09993] *** End of error message ***
</pre>
{% endraw %}
