**Project ID:** [plumID:25.023]({{ '/' | absolute_url }}eggs/25/023/)  
Stderr for source:  update_2026/initial_relaxed_conf_for_metad/dimer/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(colvar/RMSDShortcut.cpp:80) PLMD::colvar::RMSDShortcut::RMSDShortcut(const PLMD::ActionOptions&)
missing file prot_ref_a.pdb
[runnervm1li68:04919] *** Process received signal ***
[runnervm1li68:04919] Signal: Aborted (6)
[runnervm1li68:04919] Signal code:  (-6)
[runnervm1li68:04919] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f363fe45330]
[runnervm1li68:04919] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f363fe9eb2c]
[runnervm1li68:04919] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f363fe4527e]
[runnervm1li68:04919] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f363fe288ff]
[runnervm1li68:04919] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f36402a5ff5]
[runnervm1li68:04919] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f36402bb0da]
[runnervm1li68:04919] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f36402a5a55]
[runnervm1li68:04919] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f36402a5a6f]
[runnervm1li68:04919] [ 8] plumed_master(+0x146dd)[0x56092cd3f6dd]
[runnervm1li68:04919] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f363fe2a1ca]
[runnervm1li68:04919] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f363fe2a28b]
[runnervm1li68:04919] [11] plumed_master(+0x15365)[0x56092cd40365]
[runnervm1li68:04919] *** End of error message ***
</pre>
{% endraw %}
