**Project ID:** [plumID:20.018]({{ '/' | absolute_url }}eggs/20/018/)  
Stderr for source:  na/plumed.inp   
Download: [zipped raw stdout](plumed.inp.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.inp.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
Assembler messages:
Fatal error: can't create plumed_mklib.mlLvo7/../src/bias/ReweightGeomFES.o: No such file or directory
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:1494) void PLMD::PlumedMain::load(const std::string&)
An error happened while executing command env PLUMED_ROOT='/home/runner/opt/lib/plumed_master' PLUMED_VERSION='2.11.0-dev' PLUMED_HTMLDIR='/home/runner/opt/share/doc/plumed_master' PLUMED_INCLUDEDIR='/home/runner/opt/include' PLUMED_PROGRAM_NAME='plumed_master' PLUMED_IS_INSTALLED='yes' "/home/runner/opt/lib/plumed_master"/scripts/mklib.sh -n -o ./../src/bias/ReweightGeomFES.2.11.0-dev.so ../src/bias/ReweightGeomFES.cpp

[runnervm1li68:11715] *** Process received signal ***
[runnervm1li68:11715] Signal: Aborted (6)
[runnervm1li68:11715] Signal code:  (-6)
[runnervm1li68:11715] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f2bb4a45330]
[runnervm1li68:11715] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f2bb4a9eb2c]
[runnervm1li68:11715] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f2bb4a4527e]
[runnervm1li68:11715] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f2bb4a288ff]
[runnervm1li68:11715] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f2bb4ea5ff5]
[runnervm1li68:11715] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f2bb4ebb0da]
[runnervm1li68:11715] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f2bb4ea5a55]
[runnervm1li68:11715] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f2bb4ea5a6f]
[runnervm1li68:11715] [ 8] plumed_master(+0x146dd)[0x55c035d926dd]
[runnervm1li68:11715] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f2bb4a2a1ca]
[runnervm1li68:11715] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f2bb4a2a28b]
[runnervm1li68:11715] [11] plumed_master(+0x15365)[0x55c035d93365]
[runnervm1li68:11715] *** End of error message ***
</pre>
{% endraw %}
