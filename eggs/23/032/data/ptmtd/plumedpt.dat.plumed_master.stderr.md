**Project ID:** [plumID:23.032]({{ '/' | absolute_url }}eggs/23/032/)  
Stderr for source:  ptmtd/plumedpt.dat   
Download: [zipped raw stdout](plumedpt.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumedpt.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "PYTORCH_MODEL_CV" is not known.
[fv-az1947-39:07709] *** Process received signal ***
[fv-az1947-39:07709] Signal: Aborted (6)
[fv-az1947-39:07709] Signal code:  (-6)
[fv-az1947-39:07709] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f53bc445330]
[fv-az1947-39:07709] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f53bc49eb2c]
[fv-az1947-39:07709] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f53bc44527e]
[fv-az1947-39:07709] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f53bc4288ff]
[fv-az1947-39:07709] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f53bc8a5ff5]
[fv-az1947-39:07709] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f53bc8bb0da]
[fv-az1947-39:07709] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f53bc8a5a55]
[fv-az1947-39:07709] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f53bc8a5a6f]
[fv-az1947-39:07709] [ 8] plumed_master(+0x146dd)[0x55bb63b766dd]
[fv-az1947-39:07709] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f53bc42a1ca]
[fv-az1947-39:07709] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f53bc42a28b]
[fv-az1947-39:07709] [11] plumed_master(+0x15365)[0x55bb63b77365]
[fv-az1947-39:07709] *** End of error message ***
</pre>
{% endraw %}
