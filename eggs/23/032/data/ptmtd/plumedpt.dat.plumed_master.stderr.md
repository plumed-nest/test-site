**Project ID:** [plumID:23.032]({{ '/' | absolute_url }}eggs/23/032/)  
Stderr for source:  ptmtd/plumedpt.dat   
Download: [zipped raw stdout](plumedpt.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumedpt.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "PYTORCH_MODEL_CV" is not known.
[runnervm7b5n9:06356] *** Process received signal ***
[runnervm7b5n9:06356] Signal: Aborted (6)
[runnervm7b5n9:06356] Signal code:  (-6)
[runnervm7b5n9:06356] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fe91ac45330]
[runnervm7b5n9:06356] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fe91ac9eb2c]
[runnervm7b5n9:06356] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fe91ac4527e]
[runnervm7b5n9:06356] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fe91ac288ff]
[runnervm7b5n9:06356] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fe91b0a5ff5]
[runnervm7b5n9:06356] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fe91b0bb0da]
[runnervm7b5n9:06356] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fe91b0a5a55]
[runnervm7b5n9:06356] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fe91b0a5a6f]
[runnervm7b5n9:06356] [ 8] plumed_master(+0x146dd)[0x5579719a86dd]
[runnervm7b5n9:06356] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fe91ac2a1ca]
[runnervm7b5n9:06356] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fe91ac2a28b]
[runnervm7b5n9:06356] [11] plumed_master(+0x15365)[0x5579719a9365]
[runnervm7b5n9:06356] *** End of error message ***
</pre>
{% endraw %}
