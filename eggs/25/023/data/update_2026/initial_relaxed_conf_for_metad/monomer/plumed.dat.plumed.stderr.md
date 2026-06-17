**Project ID:** [plumID:25.023]({{ '/' | absolute_url }}eggs/25/023/)  
Stderr for source:  update_2026/initial_relaxed_conf_for_metad/monomer/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(colvar/RMSDShortcut.cpp:67) PLMD::colvar::RMSDShortcut::RMSDShortcut(const PLMD::ActionOptions&)
missing file prot_ref_a.pdb
[runnervm1li68:04954] *** Process received signal ***
[runnervm1li68:04954] Signal: Aborted (6)
[runnervm1li68:04954] Signal code:  (-6)
[runnervm1li68:04954] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f06bd645330]
[runnervm1li68:04954] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f06bd69eb2c]
[runnervm1li68:04954] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f06bd64527e]
[runnervm1li68:04954] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f06bd6288ff]
[runnervm1li68:04954] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f06bdaa5ff5]
[runnervm1li68:04954] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f06bdabb0da]
[runnervm1li68:04954] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f06bdaa5a55]
[runnervm1li68:04954] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f06bdaa5a6f]
[runnervm1li68:04954] [ 8] plumed(+0x146dd)[0x55ec82de26dd]
[runnervm1li68:04954] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f06bd62a1ca]
[runnervm1li68:04954] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f06bd62a28b]
[runnervm1li68:04954] [11] plumed(+0x15365)[0x55ec82de3365]
[runnervm1li68:04954] *** End of error message ***
</pre>
{% endraw %}
