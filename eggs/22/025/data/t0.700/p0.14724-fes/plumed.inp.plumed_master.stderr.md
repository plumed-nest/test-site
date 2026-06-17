**Project ID:** [plumID:22.025]({{ '/' | absolute_url }}eggs/22/025/)  
Stderr for source:  t0.700/p0.14724-fes/plumed.inp   
Download: [zipped raw stdout](plumed.inp.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.inp.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
Assembler messages:
Fatal error: can't create plumed_mklib.RRSoVv/../../code/ReweightGeomFES.o: No such file or directory
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:1494) void PLMD::PlumedMain::load(const std::string&)
An error happened while executing command env PLUMED_ROOT='/home/runner/opt/lib/plumed_master' PLUMED_VERSION='2.11.0-dev' PLUMED_HTMLDIR='/home/runner/opt/share/doc/plumed_master' PLUMED_INCLUDEDIR='/home/runner/opt/include' PLUMED_PROGRAM_NAME='plumed_master' PLUMED_IS_INSTALLED='yes' "/home/runner/opt/lib/plumed_master"/scripts/mklib.sh -n -o ./../../code/ReweightGeomFES.2.11.0-dev.so ../../code/ReweightGeomFES.cpp

[runnervm7b5n9:08095] *** Process received signal ***
[runnervm7b5n9:08095] Signal: Aborted (6)
[runnervm7b5n9:08095] Signal code:  (-6)
[runnervm7b5n9:08095] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f22baa45330]
[runnervm7b5n9:08095] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f22baa9eb2c]
[runnervm7b5n9:08095] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f22baa4527e]
[runnervm7b5n9:08095] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f22baa288ff]
[runnervm7b5n9:08095] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f22baea5ff5]
[runnervm7b5n9:08095] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f22baebb0da]
[runnervm7b5n9:08095] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f22baea5a55]
[runnervm7b5n9:08095] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f22baea5a6f]
[runnervm7b5n9:08095] [ 8] plumed_master(+0x146dd)[0x5651f2ce46dd]
[runnervm7b5n9:08095] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f22baa2a1ca]
[runnervm7b5n9:08095] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f22baa2a28b]
[runnervm7b5n9:08095] [11] plumed_master(+0x15365)[0x5651f2ce5365]
[runnervm7b5n9:08095] *** End of error message ***
</pre>
{% endraw %}
