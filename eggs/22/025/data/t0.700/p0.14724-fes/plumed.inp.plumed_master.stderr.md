**Project ID:** [plumID:22.025]({{ '/' | absolute_url }}eggs/22/025/)  
Stderr for source:  t0.700/p0.14724-fes/plumed.inp   
Download: [zipped raw stdout](plumed.inp.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.inp.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
Assembler messages:
Fatal error: can't create plumed_mklib.sgxo1B/../../code/ReweightGeomFES.o: No such file or directory
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:1282) void PLMD::PlumedMain::load(const string&)
An error happened while executing command env PLUMED_ROOT='/home/runner/opt/lib/plumed_master' PLUMED_VERSION='2.10.0-dev' PLUMED_HTMLDIR='/home/runner/opt/share/doc/plumed_master' PLUMED_INCLUDEDIR='/home/runner/opt/include' PLUMED_PROGRAM_NAME='plumed_master' PLUMED_IS_INSTALLED='yes' "/home/runner/opt/lib/plumed_master"/scripts/mklib.sh -n -o ./../../code/ReweightGeomFES.2.10.0-dev.so ../../code/ReweightGeomFES.cpp

[fv-az1106-239:41346] *** Process received signal ***
[fv-az1106-239:41346] Signal: Aborted (6)
[fv-az1106-239:41346] Signal code:  (-6)
[fv-az1106-239:41346] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fa886a42520]
[fv-az1106-239:41346] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fa886a969fc]
[fv-az1106-239:41346] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fa886a42476]
[fv-az1106-239:41346] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fa886a287f3]
[fv-az1106-239:41346] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fa886ea2b9e]
[fv-az1106-239:41346] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fa886eae20c]
[fv-az1106-239:41346] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fa886eae277]
[fv-az1106-239:41346] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fa886eae52b]
[fv-az1106-239:41346] [ 8] plumed_master(+0x14274)[0x56292f563274]
[fv-az1106-239:41346] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fa886a29d90]
[fv-az1106-239:41346] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fa886a29e40]
[fv-az1106-239:41346] [11] plumed_master(+0x14ed5)[0x56292f563ed5]
[fv-az1106-239:41346] *** End of error message ***
</pre>
{% endraw %}
