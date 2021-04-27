**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_2prime-2/g1-w21-s7.963/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:704, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: HILLS RESTART HEIGHT 0.000 W_STRIDE 50
Maybe a missing space or a typo?
[fv-az99-305:11146] *** Process received signal ***
[fv-az99-305:11146] Signal: Aborted (6)
[fv-az99-305:11146] Signal code:  (-6)
[fv-az99-305:11146] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fe2aac52210]
[fv-az99-305:11146] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fe2aac5218b]
[fv-az99-305:11146] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fe2aac31859]
[fv-az99-305:11146] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fe2aaeb9951]
[fv-az99-305:11146] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fe2aaec547c]
[fv-az99-305:11146] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fe2aaec54e7]
[fv-az99-305:11146] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7fe2aaec57ed]
[fv-az99-305:11146] [ 7] plumed_master(+0xf568)[0x563922839568]
[fv-az99-305:11146] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fe2aac330b3]
[fv-az99-305:11146] [ 9] plumed_master(+0xf79e)[0x56392283979e]
[fv-az99-305:11146] *** End of error message ***
</pre>
{% endraw %}
