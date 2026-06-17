**Project ID:** [plumID:22.025]({{ '/' | absolute_url }}eggs/22/025/)  
Stderr for source:  p0.026/t0.8640-fes/plumed.inp   
Download: [zipped raw stdout](plumed.inp.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.inp.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
Assembler messages:
Fatal error: can't create plumed_mklib.4PSM1i/../../code/ReweightGeomFES.o: No such file or directory
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:1494) void PLMD::PlumedMain::load(const std::string&)
An error happened while executing command env PLUMED_ROOT='/home/runner/opt/lib/plumed' PLUMED_VERSION='2.10.0' PLUMED_HTMLDIR='/home/runner/opt/share/doc/plumed' PLUMED_INCLUDEDIR='/home/runner/opt/include' PLUMED_PROGRAM_NAME='plumed' PLUMED_IS_INSTALLED='yes' "/home/runner/opt/lib/plumed"/scripts/mklib.sh -n -o ./../../code/ReweightGeomFES.2.10.0.so ../../code/ReweightGeomFES.cpp

[runnervm7b5n9:07383] *** Process received signal ***
[runnervm7b5n9:07383] Signal: Aborted (6)
[runnervm7b5n9:07383] Signal code:  (-6)
[runnervm7b5n9:07383] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f3a41845330]
[runnervm7b5n9:07383] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f3a4189eb2c]
[runnervm7b5n9:07383] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f3a4184527e]
[runnervm7b5n9:07383] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f3a418288ff]
[runnervm7b5n9:07383] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f3a41ca5ff5]
[runnervm7b5n9:07383] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f3a41cbb0da]
[runnervm7b5n9:07383] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f3a41ca5a55]
[runnervm7b5n9:07383] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f3a41ca5a6f]
[runnervm7b5n9:07383] [ 8] plumed(+0x146dd)[0x56315375a6dd]
[runnervm7b5n9:07383] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f3a4182a1ca]
[runnervm7b5n9:07383] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f3a4182a28b]
[runnervm7b5n9:07383] [11] plumed(+0x15365)[0x56315375b365]
[runnervm7b5n9:07383] *** End of error message ***
</pre>
{% endraw %}
