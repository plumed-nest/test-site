**Project ID:** [plumID:25.023]({{ '/' | absolute_url }}eggs/25/023/)  
Stderr for source:  update_2026/initial_relaxed_conf_for_metad/trimer/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(colvar/RMSDShortcut.cpp:67) PLMD::colvar::RMSDShortcut::RMSDShortcut(const PLMD::ActionOptions&)
missing file prot_ref_a.pdb
[runnervm1li68:05109] *** Process received signal ***
[runnervm1li68:05109] Signal: Aborted (6)
[runnervm1li68:05109] Signal code:  (-6)
[runnervm1li68:05109] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f3cd9c45330]
[runnervm1li68:05109] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f3cd9c9eb2c]
[runnervm1li68:05109] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f3cd9c4527e]
[runnervm1li68:05109] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f3cd9c288ff]
[runnervm1li68:05109] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f3cda0a5ff5]
[runnervm1li68:05109] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f3cda0bb0da]
[runnervm1li68:05109] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f3cda0a5a55]
[runnervm1li68:05109] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f3cda0a5a6f]
[runnervm1li68:05109] [ 8] plumed(+0x146dd)[0x557e046866dd]
[runnervm1li68:05109] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f3cd9c2a1ca]
[runnervm1li68:05109] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f3cd9c2a28b]
[runnervm1li68:05109] [11] plumed(+0x15365)[0x557e04687365]
[runnervm1li68:05109] *** End of error message ***
</pre>
{% endraw %}
