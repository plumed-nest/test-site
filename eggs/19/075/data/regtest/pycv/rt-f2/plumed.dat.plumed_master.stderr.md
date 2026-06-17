**Project ID:** [plumID:19.075]({{ '/' | absolute_url }}eggs/19/075/)  
Stderr for source:  regtest/pycv/rt-f2/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "PYTHONFUNCTION" is not known.
[runnervm7b5n9:10721] *** Process received signal ***
[runnervm7b5n9:10721] Signal: Aborted (6)
[runnervm7b5n9:10721] Signal code:  (-6)
[runnervm7b5n9:10721] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f0d34e45330]
[runnervm7b5n9:10721] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f0d34e9eb2c]
[runnervm7b5n9:10721] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f0d34e4527e]
[runnervm7b5n9:10721] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f0d34e288ff]
[runnervm7b5n9:10721] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f0d352a5ff5]
[runnervm7b5n9:10721] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f0d352bb0da]
[runnervm7b5n9:10721] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f0d352a5a55]
[runnervm7b5n9:10721] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f0d352a5a6f]
[runnervm7b5n9:10721] [ 8] plumed_master(+0x146dd)[0x55c76570a6dd]
[runnervm7b5n9:10721] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f0d34e2a1ca]
[runnervm7b5n9:10721] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f0d34e2a28b]
[runnervm7b5n9:10721] [11] plumed_master(+0x15365)[0x55c76570b365]
[runnervm7b5n9:10721] *** End of error message ***
</pre>
{% endraw %}
