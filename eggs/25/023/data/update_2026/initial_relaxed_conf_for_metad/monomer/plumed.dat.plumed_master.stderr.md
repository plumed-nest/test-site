**Project ID:** [plumID:25.023]({{ '/' | absolute_url }}eggs/25/023/)  
Stderr for source:  update_2026/initial_relaxed_conf_for_metad/monomer/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(colvar/RMSDShortcut.cpp:80) PLMD::colvar::RMSDShortcut::RMSDShortcut(const PLMD::ActionOptions&)
missing file prot_ref_a.pdb
[runnervm1li68:04971] *** Process received signal ***
[runnervm1li68:04971] Signal: Aborted (6)
[runnervm1li68:04971] Signal code:  (-6)
[runnervm1li68:04971] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f88c0c45330]
[runnervm1li68:04971] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f88c0c9eb2c]
[runnervm1li68:04971] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f88c0c4527e]
[runnervm1li68:04971] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f88c0c288ff]
[runnervm1li68:04971] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f88c10a5ff5]
[runnervm1li68:04971] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f88c10bb0da]
[runnervm1li68:04971] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f88c10a5a55]
[runnervm1li68:04971] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f88c10a5a6f]
[runnervm1li68:04971] [ 8] plumed_master(+0x146dd)[0x55da058656dd]
[runnervm1li68:04971] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f88c0c2a1ca]
[runnervm1li68:04971] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f88c0c2a28b]
[runnervm1li68:04971] [11] plumed_master(+0x15365)[0x55da05866365]
[runnervm1li68:04971] *** End of error message ***
</pre>
{% endraw %}
