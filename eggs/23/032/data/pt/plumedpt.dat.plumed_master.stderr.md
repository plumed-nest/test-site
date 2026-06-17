**Project ID:** [plumID:23.032]({{ '/' | absolute_url }}eggs/23/032/)  
Stderr for source:  pt/plumedpt.dat   
Download: [zipped raw stdout](plumedpt.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumedpt.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "PYTORCH_MODEL_CV" is not known.
[runnervm7b5n9:06302] *** Process received signal ***
[runnervm7b5n9:06302] Signal: Aborted (6)
[runnervm7b5n9:06302] Signal code:  (-6)
[runnervm7b5n9:06302] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fe7b9845330]
[runnervm7b5n9:06302] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fe7b989eb2c]
[runnervm7b5n9:06302] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fe7b984527e]
[runnervm7b5n9:06302] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fe7b98288ff]
[runnervm7b5n9:06302] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fe7b9ca5ff5]
[runnervm7b5n9:06302] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fe7b9cbb0da]
[runnervm7b5n9:06302] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fe7b9ca5a55]
[runnervm7b5n9:06302] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fe7b9ca5a6f]
[runnervm7b5n9:06302] [ 8] plumed_master(+0x146dd)[0x5621b2fda6dd]
[runnervm7b5n9:06302] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fe7b982a1ca]
[runnervm7b5n9:06302] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fe7b982a28b]
[runnervm7b5n9:06302] [11] plumed_master(+0x15365)[0x5621b2fdb365]
[runnervm7b5n9:06302] *** End of error message ***
</pre>
{% endraw %}
