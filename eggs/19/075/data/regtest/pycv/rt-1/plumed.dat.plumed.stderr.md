**Project ID:** [plumID:19.075]({{ '/' | absolute_url }}eggs/19/075/)  
Stderr for source:  regtest/pycv/rt-1/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "PYTHONCV" is not known.
[runnervm7b5n9:10499] *** Process received signal ***
[runnervm7b5n9:10499] Signal: Aborted (6)
[runnervm7b5n9:10499] Signal code:  (-6)
[runnervm7b5n9:10499] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f1d7b845330]
[runnervm7b5n9:10499] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f1d7b89eb2c]
[runnervm7b5n9:10499] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f1d7b84527e]
[runnervm7b5n9:10499] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f1d7b8288ff]
[runnervm7b5n9:10499] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f1d7bca5ff5]
[runnervm7b5n9:10499] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f1d7bcbb0da]
[runnervm7b5n9:10499] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f1d7bca5a55]
[runnervm7b5n9:10499] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f1d7bca5a6f]
[runnervm7b5n9:10499] [ 8] plumed(+0x146dd)[0x560e2031e6dd]
[runnervm7b5n9:10499] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f1d7b82a1ca]
[runnervm7b5n9:10499] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f1d7b82a28b]
[runnervm7b5n9:10499] [11] plumed(+0x15365)[0x560e2031f365]
[runnervm7b5n9:10499] *** End of error message ***
</pre>
{% endraw %}
