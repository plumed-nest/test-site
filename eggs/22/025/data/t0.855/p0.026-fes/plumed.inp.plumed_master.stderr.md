**Project ID:** [plumID:22.025]({{ '/' | absolute_url }}eggs/22/025/)  
Stderr for source:  t0.855/p0.026-fes/plumed.inp   
Download: [zipped raw stdout](plumed.inp.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.inp.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
Assembler messages:
Fatal error: can't create plumed_mklib.xfRLzL/../../code/ReweightGeomFES.o: No such file or directory
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:1494) void PLMD::PlumedMain::load(const std::string&)
An error happened while executing command env PLUMED_ROOT='/home/runner/opt/lib/plumed_master' PLUMED_VERSION='2.11.0-dev' PLUMED_HTMLDIR='/home/runner/opt/share/doc/plumed_master' PLUMED_INCLUDEDIR='/home/runner/opt/include' PLUMED_PROGRAM_NAME='plumed_master' PLUMED_IS_INSTALLED='yes' "/home/runner/opt/lib/plumed_master"/scripts/mklib.sh -n -o ./../../code/ReweightGeomFES.2.11.0-dev.so ../../code/ReweightGeomFES.cpp

[runnervm7b5n9:08357] *** Process received signal ***
[runnervm7b5n9:08357] Signal: Aborted (6)
[runnervm7b5n9:08357] Signal code:  (-6)
[runnervm7b5n9:08357] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f7799645330]
[runnervm7b5n9:08357] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f779969eb2c]
[runnervm7b5n9:08357] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f779964527e]
[runnervm7b5n9:08357] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f77996288ff]
[runnervm7b5n9:08357] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f7799aa5ff5]
[runnervm7b5n9:08357] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f7799abb0da]
[runnervm7b5n9:08357] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f7799aa5a55]
[runnervm7b5n9:08357] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f7799aa5a6f]
[runnervm7b5n9:08357] [ 8] plumed_master(+0x146dd)[0x5555828e16dd]
[runnervm7b5n9:08357] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f779962a1ca]
[runnervm7b5n9:08357] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f779962a28b]
[runnervm7b5n9:08357] [11] plumed_master(+0x15365)[0x5555828e2365]
[runnervm7b5n9:08357] *** End of error message ***
</pre>
{% endraw %}
