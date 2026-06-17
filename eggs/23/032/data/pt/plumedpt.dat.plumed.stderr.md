**Project ID:** [plumID:23.032]({{ '/' | absolute_url }}eggs/23/032/)  
Stderr for source:  pt/plumedpt.dat   
Download: [zipped raw stdout](plumedpt.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumedpt.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "PYTORCH_MODEL_CV" is not known.
[runnervm7b5n9:06287] *** Process received signal ***
[runnervm7b5n9:06287] Signal: Aborted (6)
[runnervm7b5n9:06287] Signal code:  (-6)
[runnervm7b5n9:06287] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fe6c8045330]
[runnervm7b5n9:06287] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fe6c809eb2c]
[runnervm7b5n9:06287] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fe6c804527e]
[runnervm7b5n9:06287] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fe6c80288ff]
[runnervm7b5n9:06287] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fe6c84a5ff5]
[runnervm7b5n9:06287] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fe6c84bb0da]
[runnervm7b5n9:06287] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fe6c84a5a55]
[runnervm7b5n9:06287] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fe6c84a5a6f]
[runnervm7b5n9:06287] [ 8] plumed(+0x146dd)[0x563d53c8a6dd]
[runnervm7b5n9:06287] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fe6c802a1ca]
[runnervm7b5n9:06287] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fe6c802a28b]
[runnervm7b5n9:06287] [11] plumed(+0x15365)[0x563d53c8b365]
[runnervm7b5n9:06287] *** End of error message ***
</pre>
{% endraw %}
