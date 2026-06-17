**Project ID:** [plumID:19.046]({{ '/' | absolute_url }}eggs/19/046/)  
Stderr for source:  PLUMED_FM/plumed_FM.dat   
Download: [zipped raw stdout](plumed_FM.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_FM.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "FPS" is not known.
[runnervm7b5n9:11791] *** Process received signal ***
[runnervm7b5n9:11791] Signal: Aborted (6)
[runnervm7b5n9:11791] Signal code:  (-6)
[runnervm7b5n9:11791] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f79f6445330]
[runnervm7b5n9:11791] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f79f649eb2c]
[runnervm7b5n9:11791] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f79f644527e]
[runnervm7b5n9:11791] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f79f64288ff]
[runnervm7b5n9:11791] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f79f68a5ff5]
[runnervm7b5n9:11791] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f79f68bb0da]
[runnervm7b5n9:11791] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f79f68a5a55]
[runnervm7b5n9:11791] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f79f68a5a6f]
[runnervm7b5n9:11791] [ 8] plumed_master(+0x146dd)[0x55aaac24a6dd]
[runnervm7b5n9:11791] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f79f642a1ca]
[runnervm7b5n9:11791] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f79f642a28b]
[runnervm7b5n9:11791] [11] plumed_master(+0x15365)[0x55aaac24b365]
[runnervm7b5n9:11791] *** End of error message ***
</pre>
{% endraw %}
