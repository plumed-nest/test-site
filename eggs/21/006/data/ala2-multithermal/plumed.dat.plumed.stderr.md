**Project ID:** [plumID:21.006]({{ '/' | absolute_url }}eggs/21/006/)  
Stderr for source:  ala2-multithermal/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:706, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: ECV_MULTITHERMAL LABEL=ecv ARG=ene MAX_TEMP=1000 STEPS_TEMP=4
Maybe a missing space or a typo?
[fv-az99-305:17539] *** Process received signal ***
[fv-az99-305:17539] Signal: Aborted (6)
[fv-az99-305:17539] Signal code:  (-6)
[fv-az99-305:17539] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7ff058968210]
[fv-az99-305:17539] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7ff05896818b]
[fv-az99-305:17539] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7ff058947859]
[fv-az99-305:17539] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7ff058bcf951]
[fv-az99-305:17539] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7ff058bdb47c]
[fv-az99-305:17539] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7ff058bdb4e7]
[fv-az99-305:17539] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7ff058bdb799]
[fv-az99-305:17539] [ 7] plumed(+0xf47d)[0x55be075aa47d]
[fv-az99-305:17539] [ 8] plumed(+0x14004)[0x55be075af004]
[fv-az99-305:17539] [ 9] plumed(+0xf698)[0x55be075aa698]
[fv-az99-305:17539] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7ff0589490b3]
[fv-az99-305:17539] [11] plumed(+0xf76e)[0x55be075aa76e]
[fv-az99-305:17539] *** End of error message ***
</pre>
{% endraw %}
