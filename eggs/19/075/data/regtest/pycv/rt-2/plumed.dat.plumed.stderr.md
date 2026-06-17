**Project ID:** [plumID:19.075]({{ '/' | absolute_url }}eggs/19/075/)  
Stderr for source:  regtest/pycv/rt-2/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "PYTHONCV" is not known.
[runnervm7b5n9:10552] *** Process received signal ***
[runnervm7b5n9:10552] Signal: Aborted (6)
[runnervm7b5n9:10552] Signal code:  (-6)
[runnervm7b5n9:10552] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fe3a9045330]
[runnervm7b5n9:10552] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fe3a909eb2c]
[runnervm7b5n9:10552] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fe3a904527e]
[runnervm7b5n9:10552] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fe3a90288ff]
[runnervm7b5n9:10552] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fe3a94a5ff5]
[runnervm7b5n9:10552] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fe3a94bb0da]
[runnervm7b5n9:10552] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fe3a94a5a55]
[runnervm7b5n9:10552] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fe3a94a5a6f]
[runnervm7b5n9:10552] [ 8] plumed(+0x146dd)[0x55ce5f6cb6dd]
[runnervm7b5n9:10552] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fe3a902a1ca]
[runnervm7b5n9:10552] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fe3a902a28b]
[runnervm7b5n9:10552] [11] plumed(+0x15365)[0x55ce5f6cc365]
[runnervm7b5n9:10552] *** End of error message ***
</pre>
{% endraw %}
