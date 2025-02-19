**Project ID:** [plumID:23.032]({{ '/' | absolute_url }}eggs/23/032/)  
Stderr for source:  pt/plumedpt.dat   
Download: [zipped raw stdout](plumedpt.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumedpt.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "PYTORCH_MODEL_CV" is not known.
[fv-az1947-39:07641] *** Process received signal ***
[fv-az1947-39:07641] Signal: Aborted (6)
[fv-az1947-39:07641] Signal code:  (-6)
[fv-az1947-39:07641] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f6220645330]
[fv-az1947-39:07641] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f622069eb2c]
[fv-az1947-39:07641] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f622064527e]
[fv-az1947-39:07641] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f62206288ff]
[fv-az1947-39:07641] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f6220aa5ff5]
[fv-az1947-39:07641] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f6220abb0da]
[fv-az1947-39:07641] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f6220aa5a55]
[fv-az1947-39:07641] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f6220aa5a6f]
[fv-az1947-39:07641] [ 8] plumed(+0x146dd)[0x5638f74b36dd]
[fv-az1947-39:07641] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f622062a1ca]
[fv-az1947-39:07641] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f622062a28b]
[fv-az1947-39:07641] [11] plumed(+0x15365)[0x5638f74b4365]
[fv-az1947-39:07641] *** End of error message ***
</pre>
{% endraw %}
