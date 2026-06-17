**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w18-s4.980/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "HILLS" is not known.
[runnervm7b5n9:08843] *** Process received signal ***
[runnervm7b5n9:08843] Signal: Aborted (6)
[runnervm7b5n9:08843] Signal code:  (-6)
[runnervm7b5n9:08843] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f22c6645330]
[runnervm7b5n9:08843] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f22c669eb2c]
[runnervm7b5n9:08843] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f22c664527e]
[runnervm7b5n9:08843] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f22c66288ff]
[runnervm7b5n9:08843] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f22c6aa5ff5]
[runnervm7b5n9:08843] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f22c6abb0da]
[runnervm7b5n9:08843] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f22c6aa5a55]
[runnervm7b5n9:08843] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f22c6aa5a6f]
[runnervm7b5n9:08843] [ 8] plumed(+0x146dd)[0x559dfeff96dd]
[runnervm7b5n9:08843] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f22c662a1ca]
[runnervm7b5n9:08843] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f22c662a28b]
[runnervm7b5n9:08843] [11] plumed(+0x15365)[0x559dfeffa365]
[runnervm7b5n9:08843] *** End of error message ***
</pre>
{% endraw %}
