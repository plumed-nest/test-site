**Project ID:** [plumID:19.075]({{ '/' | absolute_url }}eggs/19/075/)  
Stderr for source:  regtest/pycv/rt-1/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "PYTHONCV" is not known.
[runnervm7b5n9:10514] *** Process received signal ***
[runnervm7b5n9:10514] Signal: Aborted (6)
[runnervm7b5n9:10514] Signal code:  (-6)
[runnervm7b5n9:10514] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fb9f3e45330]
[runnervm7b5n9:10514] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fb9f3e9eb2c]
[runnervm7b5n9:10514] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fb9f3e4527e]
[runnervm7b5n9:10514] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fb9f3e288ff]
[runnervm7b5n9:10514] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fb9f42a5ff5]
[runnervm7b5n9:10514] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fb9f42bb0da]
[runnervm7b5n9:10514] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fb9f42a5a55]
[runnervm7b5n9:10514] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fb9f42a5a6f]
[runnervm7b5n9:10514] [ 8] plumed_master(+0x146dd)[0x56206dcf76dd]
[runnervm7b5n9:10514] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fb9f3e2a1ca]
[runnervm7b5n9:10514] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fb9f3e2a28b]
[runnervm7b5n9:10514] [11] plumed_master(+0x15365)[0x56206dcf8365]
[runnervm7b5n9:10514] *** End of error message ***
</pre>
{% endraw %}
