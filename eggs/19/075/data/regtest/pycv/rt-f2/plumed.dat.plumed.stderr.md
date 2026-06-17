**Project ID:** [plumID:19.075]({{ '/' | absolute_url }}eggs/19/075/)  
Stderr for source:  regtest/pycv/rt-f2/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "PYTHONFUNCTION" is not known.
[runnervm7b5n9:10706] *** Process received signal ***
[runnervm7b5n9:10706] Signal: Aborted (6)
[runnervm7b5n9:10706] Signal code:  (-6)
[runnervm7b5n9:10706] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f8e80c45330]
[runnervm7b5n9:10706] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f8e80c9eb2c]
[runnervm7b5n9:10706] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f8e80c4527e]
[runnervm7b5n9:10706] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f8e80c288ff]
[runnervm7b5n9:10706] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f8e810a5ff5]
[runnervm7b5n9:10706] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f8e810bb0da]
[runnervm7b5n9:10706] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f8e810a5a55]
[runnervm7b5n9:10706] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f8e810a5a6f]
[runnervm7b5n9:10706] [ 8] plumed(+0x146dd)[0x556b7fcd96dd]
[runnervm7b5n9:10706] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f8e80c2a1ca]
[runnervm7b5n9:10706] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f8e80c2a28b]
[runnervm7b5n9:10706] [11] plumed(+0x15365)[0x556b7fcda365]
[runnervm7b5n9:10706] *** End of error message ***
</pre>
{% endraw %}
