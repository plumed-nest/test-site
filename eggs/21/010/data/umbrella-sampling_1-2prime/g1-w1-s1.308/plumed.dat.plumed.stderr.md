**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w1-s1.308/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "HILLS" is not known.
[runnervm7b5n9:08379] *** Process received signal ***
[runnervm7b5n9:08379] Signal: Aborted (6)
[runnervm7b5n9:08379] Signal code:  (-6)
[runnervm7b5n9:08379] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f7140845330]
[runnervm7b5n9:08379] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f714089eb2c]
[runnervm7b5n9:08379] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f714084527e]
[runnervm7b5n9:08379] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f71408288ff]
[runnervm7b5n9:08379] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f7140ca5ff5]
[runnervm7b5n9:08379] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f7140cbb0da]
[runnervm7b5n9:08379] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f7140ca5a55]
[runnervm7b5n9:08379] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f7140ca5a6f]
[runnervm7b5n9:08379] [ 8] plumed(+0x146dd)[0x560eeb3296dd]
[runnervm7b5n9:08379] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f714082a1ca]
[runnervm7b5n9:08379] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f714082a28b]
[runnervm7b5n9:08379] [11] plumed(+0x15365)[0x560eeb32a365]
[runnervm7b5n9:08379] *** End of error message ***
</pre>
{% endraw %}
