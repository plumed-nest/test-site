**Project ID:** [plumID:21.033]({{ '/' | absolute_url }}eggs/21/033/)  
Stderr for source:  outside_path/plumed.5.dat   
Download: [zipped raw stdout](plumed.5.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.5.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
WARNING: using a legacy ActionRegister.h include path, please use <<#include "core/ActionRegister.h">>
WARNING: "core/Atoms.h" does not exist anymore in  version >=2.10, you should change your code.
../PathCV.DFoBJ7.cpp: In static member function ‘static void PLMD::function::PathCV::registerKeywords(PLMD::Keywords&)’:
../PathCV.DFoBJ7.cpp:198:3: error: ‘componentsAreNotOptional’ was not declared in this scope
198 |   componentsAreNotOptional(keys);
|   ^~~~~~~~~~~~~~~~~~~~~~~~
../PathCV.DFoBJ7.cpp: In destructor ‘virtual PLMD::function::PathCV::~PathCV()’:
../PathCV.DFoBJ7.cpp:208:16: warning: comparison of integer expressions of different signedness: ‘int’ and ‘unsigned int’ [-Wsign-compare]
208 |   for(int i=0;i<mw_n_;++i){
|               ~^~~~~~
../PathCV.DFoBJ7.cpp: In constructor ‘PLMD::function::PathCV::PathCV(const PLMD::ActionOptions&)’:
../PathCV.DFoBJ7.cpp:236:16: warning: comparison of integer expressions of different signedness: ‘int’ and ‘unsigned int’ [-Wsign-compare]
236 |   for(int i=0;i<mw_n_;++i){
|               ~^~~~~~
../PathCV.DFoBJ7.cpp:259:11: warning: comparison of integer expressions of different signedness: ‘int’ and ‘unsigned int’ [-Wsign-compare]
259 |       if(i==mw_id_) ifiles[i]->close();
|          ~^~~~~~~~
../PathCV.DFoBJ7.cpp: In member function ‘void PLMD::function::PathCV::generatePath()’:
../PathCV.DFoBJ7.cpp:483:26: warning: comparison of integer expressions of different signedness: ‘int’ and ‘unsigned int’ [-Wsign-compare]
483 |     for(int inode=0;inode<nnodes;inode++){
|                     ~~~~~^~~~~~~
../PathCV.DFoBJ7.cpp: In member function ‘void PLMD::function::PathCV::readMultipleWalkers()’:
../PathCV.DFoBJ7.cpp:941:16: warning: comparison of integer expressions of different signedness: ‘int’ and ‘unsigned int’ [-Wsign-compare]
941 |   for(int i=0;i<mw_n_;++i){
|               ~^~~~~~
../PathCV.DFoBJ7.cpp:942:9: warning: comparison of integer expressions of different signedness: ‘int’ and ‘unsigned int’ [-Wsign-compare]
942 |     if(i==mw_id_) continue;
|        ~^~~~~~~~
../PathCV.DFoBJ7.cpp:957:5: error: invalid use of incomplete type ‘class PLMD::Communicator’
957 |     comm.Barrier();
|     ^~~~
In file included from /home/runner/opt/include/plumed_master/function/../core/../tools/OFile.h:25,
from /home/runner/opt/include/plumed_master/function/../core/../tools/Log.h:25,
from /home/runner/opt/include/plumed_master/function/../core/Action.h:30,
from /home/runner/opt/include/plumed_master/function/../core/ActionWithValue.h:25,
from /home/runner/opt/include/plumed_master/function/Function.h:25,
from ../PathCV.DFoBJ7.cpp:22:
/home/runner/opt/include/plumed_master/function/../core/../tools/FileBase.h:29:7: note: forward declaration of ‘class PLMD::Communicator’
29 | class Communicator;
|       ^~~~~~~~~~~~
../PathCV.DFoBJ7.cpp:958:5: error: invalid use of incomplete type ‘class PLMD::Communicator’
958 |     multi_sim_comm.Barrier();
|     ^~~~~~~~~~~~~~
In file included from /home/runner/opt/include/plumed_master/function/../core/../tools/OFile.h:25,
from /home/runner/opt/include/plumed_master/function/../core/../tools/Log.h:25,
from /home/runner/opt/include/plumed_master/function/../core/Action.h:30,
from /home/runner/opt/include/plumed_master/function/../core/ActionWithValue.h:25,
from /home/runner/opt/include/plumed_master/function/Function.h:25,
from ../PathCV.DFoBJ7.cpp:22:
/home/runner/opt/include/plumed_master/function/../core/../tools/FileBase.h:29:7: note: forward declaration of ‘class PLMD::Communicator’
29 | class Communicator;
|       ^~~~~~~~~~~~
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:1292) void PLMD::PlumedMain::load(const string&)
An error happened while executing command env PLUMED_ROOT='/home/runner/opt/lib/plumed_master' PLUMED_VERSION='2.10.0-dev' PLUMED_HTMLDIR='/home/runner/opt/share/doc/plumed_master' PLUMED_INCLUDEDIR='/home/runner/opt/include' PLUMED_PROGRAM_NAME='plumed_master' PLUMED_IS_INSTALLED='yes' "/home/runner/opt/lib/plumed_master"/scripts/mklib.sh -n -o ./../PathCV.2.10.0-dev.so ../PathCV.cpp

[fv-az1445-962:73074] *** Process received signal ***
[fv-az1445-962:73074] Signal: Aborted (6)
[fv-az1445-962:73074] Signal code:  (-6)
[fv-az1445-962:73074] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f6355c42520]
[fv-az1445-962:73074] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f6355c969fc]
[fv-az1445-962:73074] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f6355c42476]
[fv-az1445-962:73074] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f6355c287f3]
[fv-az1445-962:73074] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f63560a2b9e]
[fv-az1445-962:73074] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f63560ae20c]
[fv-az1445-962:73074] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f63560ae277]
[fv-az1445-962:73074] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f63560ae52b]
[fv-az1445-962:73074] [ 8] plumed_master(+0x14274)[0x563d4170a274]
[fv-az1445-962:73074] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f6355c29d90]
[fv-az1445-962:73074] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f6355c29e40]
[fv-az1445-962:73074] [11] plumed_master(+0x14ed5)[0x563d4170aed5]
[fv-az1445-962:73074] *** End of error message ***
</pre>
{% endraw %}