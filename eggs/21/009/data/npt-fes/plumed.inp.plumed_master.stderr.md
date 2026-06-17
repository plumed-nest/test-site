**Project ID:** [plumID:21.009]({{ '/' | absolute_url }}eggs/21/009/)  
Stderr for source:  npt-fes/plumed.inp   
Download: [zipped raw stdout](plumed.inp.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.inp.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
Assembler messages:
Fatal error: can't create plumed_mklib.hWE8QT/../codes/ReweightGeomFES.o: No such file or directory
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:1494) void PLMD::PlumedMain::load(const std::string&)
An error happened while executing command env PLUMED_ROOT='/home/runner/opt/lib/plumed_master' PLUMED_VERSION='2.11.0-dev' PLUMED_HTMLDIR='/home/runner/opt/share/doc/plumed_master' PLUMED_INCLUDEDIR='/home/runner/opt/include' PLUMED_PROGRAM_NAME='plumed_master' PLUMED_IS_INSTALLED='yes' "/home/runner/opt/lib/plumed_master"/scripts/mklib.sh -n -o ./../codes/ReweightGeomFES.2.11.0-dev.so ../codes/ReweightGeomFES.cpp

[runnervm1li68:09522] *** Process received signal ***
[runnervm1li68:09522] Signal: Aborted (6)
[runnervm1li68:09522] Signal code:  (-6)
[runnervm1li68:09522] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f01a9045330]
[runnervm1li68:09522] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f01a909eb2c]
[runnervm1li68:09522] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f01a904527e]
[runnervm1li68:09522] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f01a90288ff]
[runnervm1li68:09522] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f01a94a5ff5]
[runnervm1li68:09522] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f01a94bb0da]
[runnervm1li68:09522] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f01a94a5a55]
[runnervm1li68:09522] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f01a94a5a6f]
[runnervm1li68:09522] [ 8] plumed_master(+0x146dd)[0x562b2aa976dd]
[runnervm1li68:09522] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f01a902a1ca]
[runnervm1li68:09522] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f01a902a28b]
[runnervm1li68:09522] [11] plumed_master(+0x15365)[0x562b2aa98365]
[runnervm1li68:09522] *** End of error message ***
</pre>
{% endraw %}
