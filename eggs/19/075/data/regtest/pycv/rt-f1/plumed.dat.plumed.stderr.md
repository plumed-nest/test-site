**Project ID:** [plumID:19.075]({{ '/' | absolute_url }}eggs/19/075/)  
Stderr for source:  regtest/pycv/rt-f1/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:706, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: PYTHONFUNCTION LABEL=dAB2 ARG=dAB IMPORT=pythonfunction FUNCTION=square PERIODIC=NO
Maybe a missing space or a typo?
[fv-az99-305:30374] *** Process received signal ***
[fv-az99-305:30374] Signal: Aborted (6)
[fv-az99-305:30374] Signal code:  (-6)
[fv-az99-305:30374] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f06d3775210]
[fv-az99-305:30374] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f06d377518b]
[fv-az99-305:30374] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f06d3754859]
[fv-az99-305:30374] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f06d39dc951]
[fv-az99-305:30374] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f06d39e847c]
[fv-az99-305:30374] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f06d39e84e7]
[fv-az99-305:30374] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f06d39e8799]
[fv-az99-305:30374] [ 7] plumed(+0xf47d)[0x562e775bb47d]
[fv-az99-305:30374] [ 8] plumed(+0x14004)[0x562e775c0004]
[fv-az99-305:30374] [ 9] plumed(+0xf698)[0x562e775bb698]
[fv-az99-305:30374] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f06d37560b3]
[fv-az99-305:30374] [11] plumed(+0xf76e)[0x562e775bb76e]
[fv-az99-305:30374] *** End of error message ***
</pre>
{% endraw %}
