**Project ID:** [plumID:19.075]({{ '/' | absolute_url }}eggs/19/075/)  
Stderr for source:  regtest/pycv/rt-jax1/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:704, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: PYTHONCV LABEL=cv1 ATOMS=1,4 IMPORT=jaxcv FUNCTION=cv1
Maybe a missing space or a typo?
[fv-az99-305:30431] *** Process received signal ***
[fv-az99-305:30431] Signal: Aborted (6)
[fv-az99-305:30431] Signal code:  (-6)
[fv-az99-305:30431] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fe55c832210]
[fv-az99-305:30431] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fe55c83218b]
[fv-az99-305:30431] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fe55c811859]
[fv-az99-305:30431] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fe55ca99951]
[fv-az99-305:30431] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fe55caa547c]
[fv-az99-305:30431] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fe55caa54e7]
[fv-az99-305:30431] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7fe55caa57ed]
[fv-az99-305:30431] [ 7] plumed_master(+0xf568)[0x561c3bc2f568]
[fv-az99-305:30431] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fe55c8130b3]
[fv-az99-305:30431] [ 9] plumed_master(+0xf79e)[0x561c3bc2f79e]
[fv-az99-305:30431] *** End of error message ***
</pre>
{% endraw %}
