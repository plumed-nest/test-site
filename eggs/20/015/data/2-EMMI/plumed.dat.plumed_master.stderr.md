**Project ID:** [plumID:20.015]({{ '/' | absolute_url }}eggs/20/015/)  
Stderr for source:  2-EMMI/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
WARNING: using a legacy ActionRegister.h include path, please use <<#include "core/ActionRegister.h">>
EMMIVox.HwYFKS.cpp: In constructor ‘PLMD::isdb::EMMIVOX::EMMIVOX(const PLMD::ActionOptions&)’:
EMMIVox.HwYFKS.cpp:327:28: error: ‘class PLMD::PlumedMain’ has no member named ‘getAtoms’
327 |   if(temp>0.0) kbt_=plumed.getAtoms().getKBoltzmann()*temp;
|                            ^~~~~~~~
EMMIVox.HwYFKS.cpp:328:20: error: ‘class PLMD::PlumedMain’ has no member named ‘getAtoms’
328 |   else kbt_=plumed.getAtoms().getKbT();
|                    ^~~~~~~~
EMMIVox.HwYFKS.cpp:376:20: error: invalid use of incomplete type ‘class PLMD::Communicator’
376 |   unsigned mpisize=comm.Get_size();
|                    ^~~~
In file included from /home/runner/opt/include/plumed_master/colvar/../core/../tools/OFile.h:25,
from /home/runner/opt/include/plumed_master/colvar/../core/../tools/Log.h:25,
from /home/runner/opt/include/plumed_master/colvar/../core/Action.h:30,
from /home/runner/opt/include/plumed_master/colvar/../core/ActionAtomistic.h:25,
from /home/runner/opt/include/plumed_master/colvar/../core/Colvar.h:25,
from /home/runner/opt/include/plumed_master/colvar/Colvar.h:24,
from EMMIVox.HwYFKS.cpp:22:
/home/runner/opt/include/plumed_master/colvar/../core/../tools/FileBase.h:29:7: note: forward declaration of ‘class PLMD::Communicator’
29 | class Communicator;
|       ^~~~~~~~~~~~
EMMIVox.HwYFKS.cpp:383:13: error: invalid use of incomplete type ‘class PLMD::Communicator’
383 |     nrep_ = multi_sim_comm.Get_size();
|             ^~~~~~~~~~~~~~
In file included from /home/runner/opt/include/plumed_master/colvar/../core/../tools/OFile.h:25,
from /home/runner/opt/include/plumed_master/colvar/../core/../tools/Log.h:25,
from /home/runner/opt/include/plumed_master/colvar/../core/Action.h:30,
from /home/runner/opt/include/plumed_master/colvar/../core/ActionAtomistic.h:25,
from /home/runner/opt/include/plumed_master/colvar/../core/Colvar.h:25,
from /home/runner/opt/include/plumed_master/colvar/Colvar.h:24,
from EMMIVox.HwYFKS.cpp:22:
/home/runner/opt/include/plumed_master/colvar/../core/../tools/FileBase.h:29:7: note: forward declaration of ‘class PLMD::Communicator’
29 | class Communicator;
|       ^~~~~~~~~~~~
EMMIVox.HwYFKS.cpp:385:14: error: invalid use of incomplete type ‘class PLMD::Communicator’
385 |   replica_ = multi_sim_comm.Get_rank();
|              ^~~~~~~~~~~~~~
In file included from /home/runner/opt/include/plumed_master/colvar/../core/../tools/OFile.h:25,
from /home/runner/opt/include/plumed_master/colvar/../core/../tools/Log.h:25,
from /home/runner/opt/include/plumed_master/colvar/../core/Action.h:30,
from /home/runner/opt/include/plumed_master/colvar/../core/ActionAtomistic.h:25,
from /home/runner/opt/include/plumed_master/colvar/../core/Colvar.h:25,
from /home/runner/opt/include/plumed_master/colvar/Colvar.h:24,
from EMMIVox.HwYFKS.cpp:22:
/home/runner/opt/include/plumed_master/colvar/../core/../tools/FileBase.h:29:7: note: forward declaration of ‘class PLMD::Communicator’
29 | class Communicator;
|       ^~~~~~~~~~~~
EMMIVox.HwYFKS.cpp: In member function ‘void PLMD::isdb::EMMIVOX::write_model_overlap(long int)’:
EMMIVox.HwYFKS.cpp:535:17: warning: comparison of integer expressions of different signedness: ‘int’ and ‘std::vector<double>::size_type’ {aka ‘long unsigned int’} [-Wsign-compare]
535 |   for(int i=0; i<ovmd_.size(); ++i) {
|                ~^~~~~~~~~~~~~
EMMIVox.HwYFKS.cpp: In member function ‘std::vector<double> PLMD::isdb::EMMIVOX::read_exp_errors(std::string)’:
EMMIVox.HwYFKS.cpp:669:26: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
669 |       for(unsigned i=0; i<nexp; ++i) {
|                         ~^~~~~
EMMIVox.HwYFKS.cpp: In member function ‘void PLMD::isdb::EMMIVOX::get_exp_data(std::string)’:
EMMIVox.HwYFKS.cpp:800:22: warning: comparison of integer expressions of different signedness: ‘__gnu_cxx::__alloc_traits<std::allocator<int>, int>::value_type’ {aka ‘int’} and ‘std::vector<std::vector<int> >::size_type’ {aka ‘long unsigned int’} [-Wsign-compare]
800 |     if(GMM_d_beta_[i]>=GMM_d_grps_.size()) error("Check Beta values");
EMMIVox.HwYFKS.cpp: In member function ‘void PLMD::isdb::EMMIVOX::doMonteCarloScale()’:
EMMIVox.HwYFKS.cpp:1082:5: error: invalid use of incomplete type ‘class PLMD::Communicator’
1082 |     multi_sim_comm.Sum(&new_scale, 1);
|     ^~~~~~~~~~~~~~
In file included from /home/runner/opt/include/plumed_master/colvar/../core/../tools/OFile.h:25,
from /home/runner/opt/include/plumed_master/colvar/../core/../tools/Log.h:25,
from /home/runner/opt/include/plumed_master/colvar/../core/Action.h:30,
from /home/runner/opt/include/plumed_master/colvar/../core/ActionAtomistic.h:25,
from /home/runner/opt/include/plumed_master/colvar/../core/Colvar.h:25,
from /home/runner/opt/include/plumed_master/colvar/Colvar.h:24,
from EMMIVox.HwYFKS.cpp:22:
/home/runner/opt/include/plumed_master/colvar/../core/../tools/FileBase.h:29:7: note: forward declaration of ‘class PLMD::Communicator’
29 | class Communicator;
|       ^~~~~~~~~~~~
EMMIVox.HwYFKS.cpp:1083:5: error: invalid use of incomplete type ‘class PLMD::Communicator’
1083 |     multi_sim_comm.Sum(&new_off, 1);
|     ^~~~~~~~~~~~~~
In file included from /home/runner/opt/include/plumed_master/colvar/../core/../tools/OFile.h:25,
from /home/runner/opt/include/plumed_master/colvar/../core/../tools/Log.h:25,
from /home/runner/opt/include/plumed_master/colvar/../core/Action.h:30,
from /home/runner/opt/include/plumed_master/colvar/../core/ActionAtomistic.h:25,
from /home/runner/opt/include/plumed_master/colvar/../core/Colvar.h:25,
from /home/runner/opt/include/plumed_master/colvar/Colvar.h:24,
from EMMIVox.HwYFKS.cpp:22:
/home/runner/opt/include/plumed_master/colvar/../core/../tools/FileBase.h:29:7: note: forward declaration of ‘class PLMD::Communicator’
29 | class Communicator;
|       ^~~~~~~~~~~~
EMMIVox.HwYFKS.cpp:1103:28: error: invalid use of incomplete type ‘class PLMD::Communicator’
1103 |   if(!no_aver_ && nrep_>1) multi_sim_comm.Sum(&new_ene, 1);
|                            ^~~~~~~~~~~~~~
In file included from /home/runner/opt/include/plumed_master/colvar/../core/../tools/OFile.h:25,
from /home/runner/opt/include/plumed_master/colvar/../core/../tools/Log.h:25,
from /home/runner/opt/include/plumed_master/colvar/../core/Action.h:30,
from /home/runner/opt/include/plumed_master/colvar/../core/ActionAtomistic.h:25,
from /home/runner/opt/include/plumed_master/colvar/../core/Colvar.h:25,
from /home/runner/opt/include/plumed_master/colvar/Colvar.h:24,
from EMMIVox.HwYFKS.cpp:22:
/home/runner/opt/include/plumed_master/colvar/../core/../tools/FileBase.h:29:7: note: forward declaration of ‘class PLMD::Communicator’
29 | class Communicator;
|       ^~~~~~~~~~~~
EMMIVox.HwYFKS.cpp:1116:5: error: invalid use of incomplete type ‘class PLMD::Communicator’
1116 |     multi_sim_comm.Sum(&do_update, 1);
|     ^~~~~~~~~~~~~~
In file included from /home/runner/opt/include/plumed_master/colvar/../core/../tools/OFile.h:25,
from /home/runner/opt/include/plumed_master/colvar/../core/../tools/Log.h:25,
from /home/runner/opt/include/plumed_master/colvar/../core/Action.h:30,
from /home/runner/opt/include/plumed_master/colvar/../core/ActionAtomistic.h:25,
from /home/runner/opt/include/plumed_master/colvar/../core/Colvar.h:25,
from /home/runner/opt/include/plumed_master/colvar/Colvar.h:24,
from EMMIVox.HwYFKS.cpp:22:
/home/runner/opt/include/plumed_master/colvar/../core/../tools/FileBase.h:29:7: note: forward declaration of ‘class PLMD::Communicator’
29 | class Communicator;
|       ^~~~~~~~~~~~
EMMIVox.HwYFKS.cpp:1127:30: error: invalid use of incomplete type ‘class PLMD::Communicator’
1127 |     if(!no_aver_ && nrep_>1) multi_sim_comm.Sum(&GMMid_der_[0], GMMid_der_.size());
|                              ^~~~~~~~~~~~~~
In file included from /home/runner/opt/include/plumed_master/colvar/../core/../tools/OFile.h:25,
from /home/runner/opt/include/plumed_master/colvar/../core/../tools/Log.h:25,
from /home/runner/opt/include/plumed_master/colvar/../core/Action.h:30,
from /home/runner/opt/include/plumed_master/colvar/../core/ActionAtomistic.h:25,
from /home/runner/opt/include/plumed_master/colvar/../core/Colvar.h:25,
from /home/runner/opt/include/plumed_master/colvar/Colvar.h:24,
from EMMIVox.HwYFKS.cpp:22:
/home/runner/opt/include/plumed_master/colvar/../core/../tools/FileBase.h:29:7: note: forward declaration of ‘class PLMD::Communicator’
29 | class Communicator;
|       ^~~~~~~~~~~~
EMMIVox.HwYFKS.cpp: In member function ‘virtual void PLMD::isdb::EMMIVOX::calculate()’:
EMMIVox.HwYFKS.cpp:1334:5: error: invalid use of incomplete type ‘class PLMD::Communicator’
1334 |     multi_sim_comm.Sum(&ovmd_[0], ovmd_.size());
|     ^~~~~~~~~~~~~~
In file included from /home/runner/opt/include/plumed_master/colvar/../core/../tools/OFile.h:25,
from /home/runner/opt/include/plumed_master/colvar/../core/../tools/Log.h:25,
from /home/runner/opt/include/plumed_master/colvar/../core/Action.h:30,
from /home/runner/opt/include/plumed_master/colvar/../core/ActionAtomistic.h:25,
from /home/runner/opt/include/plumed_master/colvar/../core/Colvar.h:25,
from /home/runner/opt/include/plumed_master/colvar/Colvar.h:24,
from EMMIVox.HwYFKS.cpp:22:
/home/runner/opt/include/plumed_master/colvar/../core/../tools/FileBase.h:29:7: note: forward declaration of ‘class PLMD::Communicator’
29 | class Communicator;
|       ^~~~~~~~~~~~
EMMIVox.HwYFKS.cpp:1383:5: error: invalid use of incomplete type ‘class PLMD::Communicator’
1383 |     multi_sim_comm.Sum(&GMMid_der_[0], GMMid_der_.size());
|     ^~~~~~~~~~~~~~
In file included from /home/runner/opt/include/plumed_master/colvar/../core/../tools/OFile.h:25,
from /home/runner/opt/include/plumed_master/colvar/../core/../tools/Log.h:25,
from /home/runner/opt/include/plumed_master/colvar/../core/Action.h:30,
from /home/runner/opt/include/plumed_master/colvar/../core/ActionAtomistic.h:25,
from /home/runner/opt/include/plumed_master/colvar/../core/Colvar.h:25,
from /home/runner/opt/include/plumed_master/colvar/Colvar.h:24,
from EMMIVox.HwYFKS.cpp:22:
/home/runner/opt/include/plumed_master/colvar/../core/../tools/FileBase.h:29:7: note: forward declaration of ‘class PLMD::Communicator’
29 | class Communicator;
|       ^~~~~~~~~~~~
EMMIVox.HwYFKS.cpp:1384:5: error: invalid use of incomplete type ‘class PLMD::Communicator’
1384 |     multi_sim_comm.Sum(&ene_, 1);
|     ^~~~~~~~~~~~~~
In file included from /home/runner/opt/include/plumed_master/colvar/../core/../tools/OFile.h:25,
from /home/runner/opt/include/plumed_master/colvar/../core/../tools/Log.h:25,
from /home/runner/opt/include/plumed_master/colvar/../core/Action.h:30,
from /home/runner/opt/include/plumed_master/colvar/../core/ActionAtomistic.h:25,
from /home/runner/opt/include/plumed_master/colvar/../core/Colvar.h:25,
from /home/runner/opt/include/plumed_master/colvar/Colvar.h:24,
from EMMIVox.HwYFKS.cpp:22:
/home/runner/opt/include/plumed_master/colvar/../core/../tools/FileBase.h:29:7: note: forward declaration of ‘class PLMD::Communicator’
29 | class Communicator;
|       ^~~~~~~~~~~~
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:1254) void PLMD::PlumedMain::load(const string&)
An error happened while executing command env PLUMED_ROOT="/home/runner/opt/lib/plumed_master" env PLUMED_VERSION="2.10.0-dev" env PLUMED_HTMLDIR="/home/runner/opt/share/doc/plumed_master" env PLUMED_INCLUDEDIR="/home/runner/opt/include" env PLUMED_PROGRAM_NAME="plumed_master" env PLUMED_IS_INSTALLED="yes" "/home/runner/opt/lib/plumed_master"/scripts/mklib.sh EMMIVox.cpp

[fv-az529-343:07974] *** Process received signal ***
[fv-az529-343:07974] Signal: Aborted (6)
[fv-az529-343:07974] Signal code:  (-6)
[fv-az529-343:07974] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f4736c42520]
[fv-az529-343:07974] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f4736c969fc]
[fv-az529-343:07974] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f4736c42476]
[fv-az529-343:07974] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f4736c287f3]
[fv-az529-343:07974] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f47370a4f26]
[fv-az529-343:07974] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f47370b6d9c]
[fv-az529-343:07974] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f47370b6e07]
[fv-az529-343:07974] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f47370b70bb]
[fv-az529-343:07974] [ 8] plumed_master(+0x12ebf)[0x55f4b966bebf]
[fv-az529-343:07974] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f4736c29d90]
[fv-az529-343:07974] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f4736c29e40]
[fv-az529-343:07974] [11] plumed_master(+0x13155)[0x55f4b966c155]
[fv-az529-343:07974] *** End of error message ***
</pre>
{% endraw %}
