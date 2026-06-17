**Project ID:** [plumID:23.026]({{ '/' | absolute_url }}eggs/23/026/)  
Stderr for source:  plumed_model_pulling.dat   
Download: [zipped raw stdout](plumed_model_pulling.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_model_pulling.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "PYTHONCV" is not known.
[runnervm7b5n9:06862] *** Process received signal ***
[runnervm7b5n9:06862] Signal: Aborted (6)
[runnervm7b5n9:06862] Signal code:  (-6)
[runnervm7b5n9:06862] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f589b645330]
[runnervm7b5n9:06862] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f589b69eb2c]
[runnervm7b5n9:06862] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f589b64527e]
[runnervm7b5n9:06862] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f589b6288ff]
[runnervm7b5n9:06862] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f589baa5ff5]
[runnervm7b5n9:06862] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f589babb0da]
[runnervm7b5n9:06862] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f589baa5a55]
[runnervm7b5n9:06862] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f589baa5a6f]
[runnervm7b5n9:06862] [ 8] plumed(+0x146dd)[0x556c2f8146dd]
[runnervm7b5n9:06862] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f589b62a1ca]
[runnervm7b5n9:06862] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f589b62a28b]
[runnervm7b5n9:06862] [11] plumed(+0x15365)[0x556c2f815365]
[runnervm7b5n9:06862] *** End of error message ***
</pre>
{% endraw %}
