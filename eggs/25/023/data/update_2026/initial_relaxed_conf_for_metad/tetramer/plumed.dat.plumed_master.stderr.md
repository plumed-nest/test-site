**Project ID:** [plumID:25.023]({{ '/' | absolute_url }}eggs/25/023/)  
Stderr for source:  update_2026/initial_relaxed_conf_for_metad/tetramer/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(colvar/RMSDShortcut.cpp:80) PLMD::colvar::RMSDShortcut::RMSDShortcut(const PLMD::ActionOptions&)
missing file prot_ref_a.pdb
[runnervm1li68:05074] *** Process received signal ***
[runnervm1li68:05074] Signal: Aborted (6)
[runnervm1li68:05074] Signal code:  (-6)
[runnervm1li68:05074] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f9441845330]
[runnervm1li68:05074] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f944189eb2c]
[runnervm1li68:05074] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f944184527e]
[runnervm1li68:05074] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f94418288ff]
[runnervm1li68:05074] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f9441ca5ff5]
[runnervm1li68:05074] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f9441cbb0da]
[runnervm1li68:05074] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f9441ca5a55]
[runnervm1li68:05074] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f9441ca5a6f]
[runnervm1li68:05074] [ 8] plumed_master(+0x146dd)[0x5578a5f1f6dd]
[runnervm1li68:05074] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f944182a1ca]
[runnervm1li68:05074] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f944182a28b]
[runnervm1li68:05074] [11] plumed_master(+0x15365)[0x5578a5f20365]
[runnervm1li68:05074] *** End of error message ***
</pre>
{% endraw %}
