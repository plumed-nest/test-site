**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w27-s6.924/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "HILLS" is not known.
[runnervm7b5n9:09357] *** Process received signal ***
[runnervm7b5n9:09357] Signal: Aborted (6)
[runnervm7b5n9:09357] Signal code:  (-6)
[runnervm7b5n9:09357] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f2b06645330]
[runnervm7b5n9:09357] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f2b0669eb2c]
[runnervm7b5n9:09357] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f2b0664527e]
[runnervm7b5n9:09357] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f2b066288ff]
[runnervm7b5n9:09357] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f2b06aa5ff5]
[runnervm7b5n9:09357] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f2b06abb0da]
[runnervm7b5n9:09357] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f2b06aa5a55]
[runnervm7b5n9:09357] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f2b06aa5a6f]
[runnervm7b5n9:09357] [ 8] plumed(+0x146dd)[0x55be3f0716dd]
[runnervm7b5n9:09357] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f2b0662a1ca]
[runnervm7b5n9:09357] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f2b0662a28b]
[runnervm7b5n9:09357] [11] plumed(+0x15365)[0x55be3f072365]
[runnervm7b5n9:09357] *** End of error message ***
</pre>
{% endraw %}
