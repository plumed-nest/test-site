**Project ID:** [plumID:22.025]({{ '/' | absolute_url }}eggs/22/025/)  
Stderr for source:  p0.026/t0.8675-fes/plumed.inp   
Download: [zipped raw stdout](plumed.inp.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.inp.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
Assembler messages:
Fatal error: can't create plumed_mklib.M7fDQi/../../code/ReweightGeomFES.o: No such file or directory
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:1292) void PLMD::PlumedMain::load(const string&)
An error happened while executing command env PLUMED_ROOT='/home/runner/opt/lib/plumed_master' PLUMED_VERSION='2.10.0-dev' PLUMED_HTMLDIR='/home/runner/opt/share/doc/plumed_master' PLUMED_INCLUDEDIR='/home/runner/opt/include' PLUMED_PROGRAM_NAME='plumed_master' PLUMED_IS_INSTALLED='yes' "/home/runner/opt/lib/plumed_master"/scripts/mklib.sh -n -o ./../../code/ReweightGeomFES.2.10.0-dev.so ../../code/ReweightGeomFES.cpp

[fv-az975-63:71296] *** Process received signal ***
[fv-az975-63:71296] Signal: Aborted (6)
[fv-az975-63:71296] Signal code:  (-6)
[fv-az975-63:71296] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7feb09a42520]
[fv-az975-63:71296] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7feb09a969fc]
[fv-az975-63:71296] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7feb09a42476]
[fv-az975-63:71296] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7feb09a287f3]
[fv-az975-63:71296] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7feb09ea2b9e]
[fv-az975-63:71296] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7feb09eae20c]
[fv-az975-63:71296] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7feb09eae277]
[fv-az975-63:71296] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7feb09eae52b]
[fv-az975-63:71296] [ 8] plumed_master(+0x14274)[0x55bab4130274]
[fv-az975-63:71296] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7feb09a29d90]
[fv-az975-63:71296] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7feb09a29e40]
[fv-az975-63:71296] [11] plumed_master(+0x14ed5)[0x55bab4130ed5]
[fv-az975-63:71296] *** End of error message ***
</pre>
{% endraw %}
