**Project ID:** [plumID:23.026]({{ '/' | absolute_url }}eggs/23/026/)  
Stderr for source:  plumed_model_pulling.dat   
Download: [zipped raw stdout](plumed_model_pulling.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_model_pulling.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "PYTHONCV" is not known.
[runnervm7b5n9:06878] *** Process received signal ***
[runnervm7b5n9:06878] Signal: Aborted (6)
[runnervm7b5n9:06878] Signal code:  (-6)
[runnervm7b5n9:06878] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f847a645330]
[runnervm7b5n9:06878] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f847a69eb2c]
[runnervm7b5n9:06878] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f847a64527e]
[runnervm7b5n9:06878] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f847a6288ff]
[runnervm7b5n9:06878] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f847aaa5ff5]
[runnervm7b5n9:06878] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f847aabb0da]
[runnervm7b5n9:06878] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f847aaa5a55]
[runnervm7b5n9:06878] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f847aaa5a6f]
[runnervm7b5n9:06878] [ 8] plumed_master(+0x146dd)[0x560ebed0e6dd]
[runnervm7b5n9:06878] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f847a62a1ca]
[runnervm7b5n9:06878] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f847a62a28b]
[runnervm7b5n9:06878] [11] plumed_master(+0x15365)[0x560ebed0f365]
[runnervm7b5n9:06878] *** End of error message ***
</pre>
{% endraw %}
