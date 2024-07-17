**Project ID:** [plumID:21.013]({{ '/' | absolute_url }}eggs/21/013/)  
Stderr for source:  h2-diss/ni001/plumed.inp   
Download: [zipped raw stdout](plumed.inp.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.inp.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
Assembler messages:
Fatal error: can't create plumed_mklib.QshTjw/../../data/ReweightGeomFES.o: No such file or directory
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:1292) void PLMD::PlumedMain::load(const string&)
An error happened while executing command env PLUMED_ROOT='/home/runner/opt/lib/plumed_master' PLUMED_VERSION='2.10.0-dev' PLUMED_HTMLDIR='/home/runner/opt/share/doc/plumed_master' PLUMED_INCLUDEDIR='/home/runner/opt/include' PLUMED_PROGRAM_NAME='plumed_master' PLUMED_IS_INSTALLED='yes' "/home/runner/opt/lib/plumed_master"/scripts/mklib.sh -n -o ./../../data/ReweightGeomFES.2.10.0-dev.so ../../data/ReweightGeomFES.cpp

[fv-az1445-962:73473] *** Process received signal ***
[fv-az1445-962:73473] Signal: Aborted (6)
[fv-az1445-962:73473] Signal code:  (-6)
[fv-az1445-962:73473] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f5b30642520]
[fv-az1445-962:73473] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f5b306969fc]
[fv-az1445-962:73473] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f5b30642476]
[fv-az1445-962:73473] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f5b306287f3]
[fv-az1445-962:73473] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f5b30aa2b9e]
[fv-az1445-962:73473] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f5b30aae20c]
[fv-az1445-962:73473] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f5b30aae277]
[fv-az1445-962:73473] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f5b30aae52b]
[fv-az1445-962:73473] [ 8] plumed_master(+0x14274)[0x55a805e3b274]
[fv-az1445-962:73473] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f5b30629d90]
[fv-az1445-962:73473] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f5b30629e40]
[fv-az1445-962:73473] [11] plumed_master(+0x14ed5)[0x55a805e3bed5]
[fv-az1445-962:73473] *** End of error message ***
</pre>
{% endraw %}
