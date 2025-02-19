**Project ID:** [plumID:21.020]({{ '/' | absolute_url }}eggs/21/020/)  
Stderr for source:  droplet/fes/plumed.inp   
Download: [zipped raw stdout](plumed.inp.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.inp.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(tools/Keywords.cpp:385) void PLMD::Keywords::use(std::string_view)
+++ assertion failed: reserved(k)
the ARG keyword is not reserved
[fv-az1770-999:07488] *** Process received signal ***
[fv-az1770-999:07488] Signal: Aborted (6)
[fv-az1770-999:07488] Signal code:  (-6)
[fv-az1770-999:07488] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fd621645330]
[fv-az1770-999:07488] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fd62169eb2c]
[fv-az1770-999:07488] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fd62164527e]
[fv-az1770-999:07488] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fd6216288ff]
[fv-az1770-999:07488] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fd621aa5ff5]
[fv-az1770-999:07488] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fd621abb0da]
[fv-az1770-999:07488] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fd621aa5a55]
[fv-az1770-999:07488] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fd621aa5a6f]
[fv-az1770-999:07488] [ 8] plumed_master(+0x146dd)[0x55e48382e6dd]
[fv-az1770-999:07488] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fd62162a1ca]
[fv-az1770-999:07488] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fd62162a28b]
[fv-az1770-999:07488] [11] plumed_master(+0x15365)[0x55e48382f365]
[fv-az1770-999:07488] *** End of error message ***
</pre>
{% endraw %}
