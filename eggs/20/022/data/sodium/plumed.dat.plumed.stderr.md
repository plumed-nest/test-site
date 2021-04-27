**Project ID:** [plumID:20.022]({{ '/' | absolute_url }}eggs/20/022/)  
Stderr for source:  sodium/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:706, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: ECV_MULTITHERMAL_MULTIBARIC LABEL=mtp ARG=ene,vol TEMP=400 MIN_TEMP=350 MAX_TEMP=450 PRESSURE=0.06022140857*5000 MIN_PRESSURE=0 MAX_PRESSURE=0.06022140857*10000
Maybe a missing space or a typo?
[fv-az99-305:22467] *** Process received signal ***
[fv-az99-305:22467] Signal: Aborted (6)
[fv-az99-305:22467] Signal code:  (-6)
[fv-az99-305:22467] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f2af5f19210]
[fv-az99-305:22467] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f2af5f1918b]
[fv-az99-305:22467] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f2af5ef8859]
[fv-az99-305:22467] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f2af6180951]
[fv-az99-305:22467] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f2af618c47c]
[fv-az99-305:22467] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f2af618c4e7]
[fv-az99-305:22467] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f2af618c799]
[fv-az99-305:22467] [ 7] plumed(+0xf47d)[0x55f83eff547d]
[fv-az99-305:22467] [ 8] plumed(+0x14004)[0x55f83effa004]
[fv-az99-305:22467] [ 9] plumed(+0xf698)[0x55f83eff5698]
[fv-az99-305:22467] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f2af5efa0b3]
[fv-az99-305:22467] [11] plumed(+0xf76e)[0x55f83eff576e]
[fv-az99-305:22467] *** End of error message ***
</pre>
{% endraw %}
