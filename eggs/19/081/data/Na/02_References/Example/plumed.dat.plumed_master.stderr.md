**Project ID:** [plumID:19.081]({{ '/' | absolute_url }}eggs/19/081/)  
Stderr for source:  Na/02_References/Example/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
../../../RefCV.MUbaeR.cpp:22:10: fatal error: multicolvar/MultiColvarBase.h: No such file or directory
22 | #include "multicolvar/MultiColvarBase.h"
|          ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
compilation terminated.
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:1282) void PLMD::PlumedMain::load(const string&)
An error happened while executing command env PLUMED_ROOT='/home/runner/opt/lib/plumed_master' PLUMED_VERSION='2.10.0-dev' PLUMED_HTMLDIR='/home/runner/opt/share/doc/plumed_master' PLUMED_INCLUDEDIR='/home/runner/opt/include' PLUMED_PROGRAM_NAME='plumed_master' PLUMED_IS_INSTALLED='yes' "/home/runner/opt/lib/plumed_master"/scripts/mklib.sh -n -o ./../../../RefCV.2.10.0-dev.so ../../../RefCV.cpp

[fv-az1435-553:43444] *** Process received signal ***
[fv-az1435-553:43444] Signal: Aborted (6)
[fv-az1435-553:43444] Signal code:  (-6)
[fv-az1435-553:43444] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fb33ae42520]
[fv-az1435-553:43444] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fb33ae969fc]
[fv-az1435-553:43444] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fb33ae42476]
[fv-az1435-553:43444] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fb33ae287f3]
[fv-az1435-553:43444] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fb33b2a2b9e]
[fv-az1435-553:43444] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fb33b2ae20c]
[fv-az1435-553:43444] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fb33b2ae277]
[fv-az1435-553:43444] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fb33b2ae52b]
[fv-az1435-553:43444] [ 8] plumed_master(+0x14274)[0x55f49a260274]
[fv-az1435-553:43444] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fb33ae29d90]
[fv-az1435-553:43444] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fb33ae29e40]
[fv-az1435-553:43444] [11] plumed_master(+0x14ed5)[0x55f49a260ed5]
[fv-az1435-553:43444] *** End of error message ***
</pre>
{% endraw %}
