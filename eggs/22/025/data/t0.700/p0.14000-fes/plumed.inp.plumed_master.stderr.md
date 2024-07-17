**Project ID:** [plumID:22.025]({{ '/' | absolute_url }}eggs/22/025/)  
Stderr for source:  t0.700/p0.14000-fes/plumed.inp   
Download: [zipped raw stdout](plumed.inp.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.inp.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
Assembler messages:
Fatal error: can't create plumed_mklib.tIF4HP/../../code/ReweightGeomFES.o: No such file or directory
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:1292) void PLMD::PlumedMain::load(const string&)
An error happened while executing command env PLUMED_ROOT='/home/runner/opt/lib/plumed_master' PLUMED_VERSION='2.10.0-dev' PLUMED_HTMLDIR='/home/runner/opt/share/doc/plumed_master' PLUMED_INCLUDEDIR='/home/runner/opt/include' PLUMED_PROGRAM_NAME='plumed_master' PLUMED_IS_INSTALLED='yes' "/home/runner/opt/lib/plumed_master"/scripts/mklib.sh -n -o ./../../code/ReweightGeomFES.2.10.0-dev.so ../../code/ReweightGeomFES.cpp

[fv-az975-63:71712] *** Process received signal ***
[fv-az975-63:71712] Signal: Aborted (6)
[fv-az975-63:71712] Signal code:  (-6)
[fv-az975-63:71712] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fb0d4442520]
[fv-az975-63:71712] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fb0d44969fc]
[fv-az975-63:71712] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fb0d4442476]
[fv-az975-63:71712] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fb0d44287f3]
[fv-az975-63:71712] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fb0d48a2b9e]
[fv-az975-63:71712] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fb0d48ae20c]
[fv-az975-63:71712] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fb0d48ae277]
[fv-az975-63:71712] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fb0d48ae52b]
[fv-az975-63:71712] [ 8] plumed_master(+0x14274)[0x557bce1c5274]
[fv-az975-63:71712] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fb0d4429d90]
[fv-az975-63:71712] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fb0d4429e40]
[fv-az975-63:71712] [11] plumed_master(+0x14ed5)[0x557bce1c5ed5]
[fv-az975-63:71712] *** End of error message ***
</pre>
{% endraw %}
