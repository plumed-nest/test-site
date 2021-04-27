**Project ID:** [plumID:21.006]({{ '/' | absolute_url }}eggs/21/006/)  
Stderr for source:  ala2-multithermal_multiumbrella/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:706, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: ECV_MULTITHERMAL LABEL=mt ARG=ene MAX_TEMP=1000 STEPS_TEMP=4
Maybe a missing space or a typo?
[fv-az99-305:17563] *** Process received signal ***
[fv-az99-305:17563] Signal: Aborted (6)
[fv-az99-305:17563] Signal code:  (-6)
[fv-az99-305:17563] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f7602d26210]
[fv-az99-305:17563] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f7602d2618b]
[fv-az99-305:17563] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f7602d05859]
[fv-az99-305:17563] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f7602f8d951]
[fv-az99-305:17563] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f7602f9947c]
[fv-az99-305:17563] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f7602f994e7]
[fv-az99-305:17563] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f7602f99799]
[fv-az99-305:17563] [ 7] plumed(+0xf47d)[0x55bf9096d47d]
[fv-az99-305:17563] [ 8] plumed(+0x14004)[0x55bf90972004]
[fv-az99-305:17563] [ 9] plumed(+0xf698)[0x55bf9096d698]
[fv-az99-305:17563] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f7602d070b3]
[fv-az99-305:17563] [11] plumed(+0xf76e)[0x55bf9096d76e]
[fv-az99-305:17563] *** End of error message ***
</pre>
{% endraw %}
