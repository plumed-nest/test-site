**Project ID:** [plumID:21.013]({{ '/' | absolute_url }}eggs/21/013/)  
Stderr for source:  ch4-diss/ni001/plumed.inp   
Download: [zipped raw stdout](plumed.inp.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.inp.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
Assembler messages:
Fatal error: can't create plumed_mklib.QM5uFL/../../data/ReweightGeomFES.o: No such file or directory
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:1494) void PLMD::PlumedMain::load(const std::string&)
An error happened while executing command env PLUMED_ROOT='/home/runner/opt/lib/plumed' PLUMED_VERSION='2.10.0' PLUMED_HTMLDIR='/home/runner/opt/share/doc/plumed' PLUMED_INCLUDEDIR='/home/runner/opt/include' PLUMED_PROGRAM_NAME='plumed' PLUMED_IS_INSTALLED='yes' "/home/runner/opt/lib/plumed"/scripts/mklib.sh -n -o ./../../data/ReweightGeomFES.2.10.0.so ../../data/ReweightGeomFES.cpp

[runnervm1li68:08465] *** Process received signal ***
[runnervm1li68:08465] Signal: Aborted (6)
[runnervm1li68:08465] Signal code:  (-6)
[runnervm1li68:08465] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7efd69045330]
[runnervm1li68:08465] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7efd6909eb2c]
[runnervm1li68:08465] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7efd6904527e]
[runnervm1li68:08465] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7efd690288ff]
[runnervm1li68:08465] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7efd694a5ff5]
[runnervm1li68:08465] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7efd694bb0da]
[runnervm1li68:08465] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7efd694a5a55]
[runnervm1li68:08465] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7efd694a5a6f]
[runnervm1li68:08465] [ 8] plumed(+0x146dd)[0x5626aeec06dd]
[runnervm1li68:08465] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7efd6902a1ca]
[runnervm1li68:08465] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7efd6902a28b]
[runnervm1li68:08465] [11] plumed(+0x15365)[0x5626aeec1365]
[runnervm1li68:08465] *** End of error message ***
</pre>
{% endraw %}
