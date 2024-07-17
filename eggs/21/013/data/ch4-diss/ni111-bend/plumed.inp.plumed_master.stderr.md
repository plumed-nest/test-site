**Project ID:** [plumID:21.013]({{ '/' | absolute_url }}eggs/21/013/)  
Stderr for source:  ch4-diss/ni111-bend/plumed.inp   
Download: [zipped raw stdout](plumed.inp.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.inp.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
Assembler messages:
Fatal error: can't create plumed_mklib.ZTjIau/../../data/ReweightGeomFES.o: No such file or directory
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:1292) void PLMD::PlumedMain::load(const string&)
An error happened while executing command env PLUMED_ROOT='/home/runner/opt/lib/plumed_master' PLUMED_VERSION='2.10.0-dev' PLUMED_HTMLDIR='/home/runner/opt/share/doc/plumed_master' PLUMED_INCLUDEDIR='/home/runner/opt/include' PLUMED_PROGRAM_NAME='plumed_master' PLUMED_IS_INSTALLED='yes' "/home/runner/opt/lib/plumed_master"/scripts/mklib.sh -n -o ./../../data/ReweightGeomFES.2.10.0-dev.so ../../data/ReweightGeomFES.cpp

[fv-az1445-962:74129] *** Process received signal ***
[fv-az1445-962:74129] Signal: Aborted (6)
[fv-az1445-962:74129] Signal code:  (-6)
[fv-az1445-962:74129] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f61b3042520]
[fv-az1445-962:74129] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f61b30969fc]
[fv-az1445-962:74129] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f61b3042476]
[fv-az1445-962:74129] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f61b30287f3]
[fv-az1445-962:74129] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f61b34a2b9e]
[fv-az1445-962:74129] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f61b34ae20c]
[fv-az1445-962:74129] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f61b34ae277]
[fv-az1445-962:74129] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f61b34ae52b]
[fv-az1445-962:74129] [ 8] plumed_master(+0x14274)[0x55e3cf4dd274]
[fv-az1445-962:74129] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f61b3029d90]
[fv-az1445-962:74129] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f61b3029e40]
[fv-az1445-962:74129] [11] plumed_master(+0x14ed5)[0x55e3cf4dded5]
[fv-az1445-962:74129] *** End of error message ***
</pre>
{% endraw %}
