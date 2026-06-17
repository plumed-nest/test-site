**Project ID:** [plumID:19.075]({{ '/' | absolute_url }}eggs/19/075/)  
Stderr for source:  regtest/pycv/rt-2/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "PYTHONCV" is not known.
[runnervm7b5n9:10568] *** Process received signal ***
[runnervm7b5n9:10568] Signal: Aborted (6)
[runnervm7b5n9:10568] Signal code:  (-6)
[runnervm7b5n9:10568] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f3d28445330]
[runnervm7b5n9:10568] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f3d2849eb2c]
[runnervm7b5n9:10568] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f3d2844527e]
[runnervm7b5n9:10568] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f3d284288ff]
[runnervm7b5n9:10568] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f3d288a5ff5]
[runnervm7b5n9:10568] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f3d288bb0da]
[runnervm7b5n9:10568] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f3d288a5a55]
[runnervm7b5n9:10568] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f3d288a5a6f]
[runnervm7b5n9:10568] [ 8] plumed_master(+0x146dd)[0x55880525e6dd]
[runnervm7b5n9:10568] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f3d2842a1ca]
[runnervm7b5n9:10568] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f3d2842a28b]
[runnervm7b5n9:10568] [11] plumed_master(+0x15365)[0x55880525f365]
[runnervm7b5n9:10568] *** End of error message ***
</pre>
{% endraw %}
