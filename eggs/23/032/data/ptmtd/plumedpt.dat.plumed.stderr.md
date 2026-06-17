**Project ID:** [plumID:23.032]({{ '/' | absolute_url }}eggs/23/032/)  
Stderr for source:  ptmtd/plumedpt.dat   
Download: [zipped raw stdout](plumedpt.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumedpt.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "PYTORCH_MODEL_CV" is not known.
[runnervm7b5n9:06341] *** Process received signal ***
[runnervm7b5n9:06341] Signal: Aborted (6)
[runnervm7b5n9:06341] Signal code:  (-6)
[runnervm7b5n9:06341] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f4f3d045330]
[runnervm7b5n9:06341] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f4f3d09eb2c]
[runnervm7b5n9:06341] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f4f3d04527e]
[runnervm7b5n9:06341] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f4f3d0288ff]
[runnervm7b5n9:06341] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f4f3d4a5ff5]
[runnervm7b5n9:06341] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f4f3d4bb0da]
[runnervm7b5n9:06341] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f4f3d4a5a55]
[runnervm7b5n9:06341] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f4f3d4a5a6f]
[runnervm7b5n9:06341] [ 8] plumed(+0x146dd)[0x56467b2826dd]
[runnervm7b5n9:06341] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f4f3d02a1ca]
[runnervm7b5n9:06341] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f4f3d02a28b]
[runnervm7b5n9:06341] [11] plumed(+0x15365)[0x56467b283365]
[runnervm7b5n9:06341] *** End of error message ***
</pre>
{% endraw %}
