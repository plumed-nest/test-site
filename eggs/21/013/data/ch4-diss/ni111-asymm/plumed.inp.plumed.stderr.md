**Project ID:** [plumID:21.013]({{ '/' | absolute_url }}eggs/21/013/)  
Stderr for source:  ch4-diss/ni111-asymm/plumed.inp   
Download: [zipped raw stdout](plumed.inp.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.inp.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
Assembler messages:
Fatal error: can't create plumed_mklib.xnZg1t/../../data/ReweightGeomFES.o: No such file or directory
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:1494) void PLMD::PlumedMain::load(const std::string&)
An error happened while executing command env PLUMED_ROOT='/home/runner/opt/lib/plumed' PLUMED_VERSION='2.10.0' PLUMED_HTMLDIR='/home/runner/opt/share/doc/plumed' PLUMED_INCLUDEDIR='/home/runner/opt/include' PLUMED_PROGRAM_NAME='plumed' PLUMED_IS_INSTALLED='yes' "/home/runner/opt/lib/plumed"/scripts/mklib.sh -n -o ./../../data/ReweightGeomFES.2.10.0.so ../../data/ReweightGeomFES.cpp

[runnervm1li68:08288] *** Process received signal ***
[runnervm1li68:08288] Signal: Aborted (6)
[runnervm1li68:08288] Signal code:  (-6)
[runnervm1li68:08288] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f73ade45330]
[runnervm1li68:08288] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f73ade9eb2c]
[runnervm1li68:08288] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f73ade4527e]
[runnervm1li68:08288] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f73ade288ff]
[runnervm1li68:08288] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f73ae2a5ff5]
[runnervm1li68:08288] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f73ae2bb0da]
[runnervm1li68:08288] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f73ae2a5a55]
[runnervm1li68:08288] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f73ae2a5a6f]
[runnervm1li68:08288] [ 8] plumed(+0x146dd)[0x558ef02236dd]
[runnervm1li68:08288] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f73ade2a1ca]
[runnervm1li68:08288] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f73ade2a28b]
[runnervm1li68:08288] [11] plumed(+0x15365)[0x558ef0224365]
[runnervm1li68:08288] *** End of error message ***
</pre>
{% endraw %}
