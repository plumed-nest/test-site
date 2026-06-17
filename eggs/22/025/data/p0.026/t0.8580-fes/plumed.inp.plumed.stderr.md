**Project ID:** [plumID:22.025]({{ '/' | absolute_url }}eggs/22/025/)  
Stderr for source:  p0.026/t0.8580-fes/plumed.inp   
Download: [zipped raw stdout](plumed.inp.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.inp.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
Assembler messages:
Fatal error: can't create plumed_mklib.CwPUwe/../../code/ReweightGeomFES.o: No such file or directory
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:1494) void PLMD::PlumedMain::load(const std::string&)
An error happened while executing command env PLUMED_ROOT='/home/runner/opt/lib/plumed' PLUMED_VERSION='2.10.0' PLUMED_HTMLDIR='/home/runner/opt/share/doc/plumed' PLUMED_INCLUDEDIR='/home/runner/opt/include' PLUMED_PROGRAM_NAME='plumed' PLUMED_IS_INSTALLED='yes' "/home/runner/opt/lib/plumed"/scripts/mklib.sh -n -o ./../../code/ReweightGeomFES.2.10.0.so ../../code/ReweightGeomFES.cpp

[runnervm7b5n9:07609] *** Process received signal ***
[runnervm7b5n9:07609] Signal: Aborted (6)
[runnervm7b5n9:07609] Signal code:  (-6)
[runnervm7b5n9:07609] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f2c5e845330]
[runnervm7b5n9:07609] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f2c5e89eb2c]
[runnervm7b5n9:07609] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f2c5e84527e]
[runnervm7b5n9:07609] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f2c5e8288ff]
[runnervm7b5n9:07609] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f2c5eca5ff5]
[runnervm7b5n9:07609] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f2c5ecbb0da]
[runnervm7b5n9:07609] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f2c5eca5a55]
[runnervm7b5n9:07609] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f2c5eca5a6f]
[runnervm7b5n9:07609] [ 8] plumed(+0x146dd)[0x55d4b8acf6dd]
[runnervm7b5n9:07609] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f2c5e82a1ca]
[runnervm7b5n9:07609] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f2c5e82a28b]
[runnervm7b5n9:07609] [11] plumed(+0x15365)[0x55d4b8ad0365]
[runnervm7b5n9:07609] *** End of error message ***
</pre>
{% endraw %}
