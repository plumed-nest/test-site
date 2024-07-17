**Project ID:** [plumID:21.009]({{ '/' | absolute_url }}eggs/21/009/)  
Stderr for source:  nvt-fes/plumed.inp   
Download: [zipped raw stdout](plumed.inp.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.inp.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
Assembler messages:
Fatal error: can't create plumed_mklib.qXlkPv/../codes/ReweightGeomFES.o: No such file or directory
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:1292) void PLMD::PlumedMain::load(const string&)
An error happened while executing command env PLUMED_ROOT='/home/runner/opt/lib/plumed_master' PLUMED_VERSION='2.10.0-dev' PLUMED_HTMLDIR='/home/runner/opt/share/doc/plumed_master' PLUMED_INCLUDEDIR='/home/runner/opt/include' PLUMED_PROGRAM_NAME='plumed_master' PLUMED_IS_INSTALLED='yes' "/home/runner/opt/lib/plumed_master"/scripts/mklib.sh -n -o ./../codes/ReweightGeomFES.2.10.0-dev.so ../codes/ReweightGeomFES.cpp

[fv-az695-456:74896] *** Process received signal ***
[fv-az695-456:74896] Signal: Aborted (6)
[fv-az695-456:74896] Signal code:  (-6)
[fv-az695-456:74896] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f4a6d842520]
[fv-az695-456:74896] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f4a6d8969fc]
[fv-az695-456:74896] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f4a6d842476]
[fv-az695-456:74896] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f4a6d8287f3]
[fv-az695-456:74896] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f4a6dca2b9e]
[fv-az695-456:74896] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f4a6dcae20c]
[fv-az695-456:74896] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f4a6dcae277]
[fv-az695-456:74896] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f4a6dcae52b]
[fv-az695-456:74896] [ 8] plumed_master(+0x14274)[0x55c84d9c6274]
[fv-az695-456:74896] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f4a6d829d90]
[fv-az695-456:74896] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f4a6d829e40]
[fv-az695-456:74896] [11] plumed_master(+0x14ed5)[0x55c84d9c6ed5]
[fv-az695-456:74896] *** End of error message ***
</pre>
{% endraw %}
