**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_5-6/g1-w10-s3.875/plumed.dat   
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
[fv-az99-305:14401] *** Process received signal ***
[fv-az99-305:14401] Signal: Aborted (6)
[fv-az99-305:14401] Signal code:  (-6)
[fv-az99-305:14401] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f690ea66210]
[fv-az99-305:14401] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f690ea6618b]
[fv-az99-305:14401] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f690ea45859]
[fv-az99-305:14401] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f690eccd951]
[fv-az99-305:14401] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f690ecd947c]
[fv-az99-305:14401] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f690ecd94e7]
[fv-az99-305:14401] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f690ecd9799]
[fv-az99-305:14401] [ 7] plumed(+0xf47d)[0x55589be4747d]
[fv-az99-305:14401] [ 8] plumed(+0x14004)[0x55589be4c004]
[fv-az99-305:14401] [ 9] plumed(+0xf698)[0x55589be47698]
[fv-az99-305:14401] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f690ea470b3]
[fv-az99-305:14401] [11] plumed(+0xf76e)[0x55589be4776e]
[fv-az99-305:14401] *** End of error message ***
</pre>
{% endraw %}
