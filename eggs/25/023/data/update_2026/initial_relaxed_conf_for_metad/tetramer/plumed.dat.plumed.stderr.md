**Project ID:** [plumID:25.023]({{ '/' | absolute_url }}eggs/25/023/)  
Stderr for source:  update_2026/initial_relaxed_conf_for_metad/tetramer/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(colvar/RMSDShortcut.cpp:67) PLMD::colvar::RMSDShortcut::RMSDShortcut(const PLMD::ActionOptions&)
missing file prot_ref_a.pdb
[runnervm1li68:05058] *** Process received signal ***
[runnervm1li68:05058] Signal: Aborted (6)
[runnervm1li68:05058] Signal code:  (-6)
[runnervm1li68:05058] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f4cc9045330]
[runnervm1li68:05058] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f4cc909eb2c]
[runnervm1li68:05058] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f4cc904527e]
[runnervm1li68:05058] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f4cc90288ff]
[runnervm1li68:05058] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f4cc94a5ff5]
[runnervm1li68:05058] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f4cc94bb0da]
[runnervm1li68:05058] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f4cc94a5a55]
[runnervm1li68:05058] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f4cc94a5a6f]
[runnervm1li68:05058] [ 8] plumed(+0x146dd)[0x557c2c9c66dd]
[runnervm1li68:05058] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f4cc902a1ca]
[runnervm1li68:05058] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f4cc902a28b]
[runnervm1li68:05058] [11] plumed(+0x15365)[0x557c2c9c7365]
[runnervm1li68:05058] *** End of error message ***
</pre>
{% endraw %}
