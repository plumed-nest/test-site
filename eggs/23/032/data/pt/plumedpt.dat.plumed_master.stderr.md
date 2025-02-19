**Project ID:** [plumID:23.032]({{ '/' | absolute_url }}eggs/23/032/)  
Stderr for source:  pt/plumedpt.dat   
Download: [zipped raw stdout](plumedpt.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumedpt.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "PYTORCH_MODEL_CV" is not known.
[fv-az1947-39:07657] *** Process received signal ***
[fv-az1947-39:07657] Signal: Aborted (6)
[fv-az1947-39:07657] Signal code:  (-6)
[fv-az1947-39:07657] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f5261645330]
[fv-az1947-39:07657] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f526169eb2c]
[fv-az1947-39:07657] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f526164527e]
[fv-az1947-39:07657] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f52616288ff]
[fv-az1947-39:07657] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f5261aa5ff5]
[fv-az1947-39:07657] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f5261abb0da]
[fv-az1947-39:07657] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f5261aa5a55]
[fv-az1947-39:07657] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f5261aa5a6f]
[fv-az1947-39:07657] [ 8] plumed_master(+0x146dd)[0x5559955bb6dd]
[fv-az1947-39:07657] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f526162a1ca]
[fv-az1947-39:07657] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f526162a28b]
[fv-az1947-39:07657] [11] plumed_master(+0x15365)[0x5559955bc365]
[fv-az1947-39:07657] *** End of error message ***
</pre>
{% endraw %}
