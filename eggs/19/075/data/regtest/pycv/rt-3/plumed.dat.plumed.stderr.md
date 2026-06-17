**Project ID:** [plumID:19.075]({{ '/' | absolute_url }}eggs/19/075/)  
Stderr for source:  regtest/pycv/rt-3/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "PYTHONCV" is not known.
[runnervm7b5n9:10604] *** Process received signal ***
[runnervm7b5n9:10604] Signal: Aborted (6)
[runnervm7b5n9:10604] Signal code:  (-6)
[runnervm7b5n9:10604] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fdc48245330]
[runnervm7b5n9:10604] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fdc4829eb2c]
[runnervm7b5n9:10604] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fdc4824527e]
[runnervm7b5n9:10604] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fdc482288ff]
[runnervm7b5n9:10604] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fdc486a5ff5]
[runnervm7b5n9:10604] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fdc486bb0da]
[runnervm7b5n9:10604] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fdc486a5a55]
[runnervm7b5n9:10604] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fdc486a5a6f]
[runnervm7b5n9:10604] [ 8] plumed(+0x146dd)[0x561468c596dd]
[runnervm7b5n9:10604] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fdc4822a1ca]
[runnervm7b5n9:10604] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fdc4822a28b]
[runnervm7b5n9:10604] [11] plumed(+0x15365)[0x561468c5a365]
[runnervm7b5n9:10604] *** End of error message ***
</pre>
{% endraw %}
