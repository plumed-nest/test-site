**Project ID:** [plumID:24.026]({{ '/' | absolute_url }}eggs/24/026/)  
Stderr for source:  CpHMD_metaD/scripts/PLUMED_GRID.dat   
Download: [zipped raw stdout](PLUMED_GRID.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](PLUMED_GRID.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(tools/Grid.cpp:655) static std::unique_ptr<PLMD::GridBase> PLMD::GridBase::create(const std::string&, const std::vector<PLMD::Value*>&, PLMD::IFile&, bool, bool, bool)
+++ assertion failed: ifile.FieldExist( funcl )
no column labelled metad.bias in in grid input
[runnervm1li68:06489] *** Process received signal ***
[runnervm1li68:06489] Signal: Aborted (6)
[runnervm1li68:06489] Signal code:  (-6)
[runnervm1li68:06489] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fcb78445330]
[runnervm1li68:06489] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fcb7849eb2c]
[runnervm1li68:06489] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fcb7844527e]
[runnervm1li68:06489] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fcb784288ff]
[runnervm1li68:06489] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fcb788a5ff5]
[runnervm1li68:06489] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fcb788bb0da]
[runnervm1li68:06489] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fcb788a5a55]
[runnervm1li68:06489] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fcb788a5a6f]
[runnervm1li68:06489] [ 8] plumed_master(+0x146dd)[0x55f9351086dd]
[runnervm1li68:06489] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fcb7842a1ca]
[runnervm1li68:06489] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fcb7842a28b]
[runnervm1li68:06489] [11] plumed_master(+0x15365)[0x55f935109365]
[runnervm1li68:06489] *** End of error message ***
</pre>
{% endraw %}
