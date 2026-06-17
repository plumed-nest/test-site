**Project ID:** [plumID:19.046]({{ '/' | absolute_url }}eggs/19/046/)  
Stderr for source:  PLUMED_FM/plumed_FM.dat   
Download: [zipped raw stdout](plumed_FM.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_FM.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "FPS" is not known.
[runnervm7b5n9:11775] *** Process received signal ***
[runnervm7b5n9:11775] Signal: Aborted (6)
[runnervm7b5n9:11775] Signal code:  (-6)
[runnervm7b5n9:11775] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f7484045330]
[runnervm7b5n9:11775] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f748409eb2c]
[runnervm7b5n9:11775] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f748404527e]
[runnervm7b5n9:11775] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f74840288ff]
[runnervm7b5n9:11775] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f74844a5ff5]
[runnervm7b5n9:11775] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f74844bb0da]
[runnervm7b5n9:11775] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f74844a5a55]
[runnervm7b5n9:11775] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f74844a5a6f]
[runnervm7b5n9:11775] [ 8] plumed(+0x146dd)[0x55eced3516dd]
[runnervm7b5n9:11775] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f748402a1ca]
[runnervm7b5n9:11775] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f748402a28b]
[runnervm7b5n9:11775] [11] plumed(+0x15365)[0x55eced352365]
[runnervm7b5n9:11775] *** End of error message ***
</pre>
{% endraw %}
