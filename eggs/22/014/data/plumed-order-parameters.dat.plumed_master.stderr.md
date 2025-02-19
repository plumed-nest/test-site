**Project ID:** [plumID:22.014]({{ '/' | absolute_url }}eggs/22/014/)  
Stderr for source:  plumed-order-parameters.dat   
Download: [zipped raw stdout](plumed-order-parameters.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed-order-parameters.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
PairEntropies.pMvPgv.cpp:22:10: fatal error: multicolvar/MultiColvarBase.h: No such file or directory
22 | #include "multicolvar/MultiColvarBase.h"
|          ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
compilation terminated.
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:1499) void PLMD::PlumedMain::load(const std::string&)
An error happened while executing command env PLUMED_ROOT='/home/runner/opt/lib/plumed_master' PLUMED_VERSION='2.11.0-dev' PLUMED_HTMLDIR='/home/runner/opt/share/doc/plumed_master' PLUMED_INCLUDEDIR='/home/runner/opt/include' PLUMED_PROGRAM_NAME='plumed_master' PLUMED_IS_INSTALLED='yes' "/home/runner/opt/lib/plumed_master"/scripts/mklib.sh -n -o ./PairEntropies.2.11.0-dev.so PairEntropies.cpp

[fv-az1947-39:08739] *** Process received signal ***
[fv-az1947-39:08739] Signal: Aborted (6)
[fv-az1947-39:08739] Signal code:  (-6)
[fv-az1947-39:08739] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fabb0245330]
[fv-az1947-39:08739] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fabb029eb2c]
[fv-az1947-39:08739] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fabb024527e]
[fv-az1947-39:08739] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fabb02288ff]
[fv-az1947-39:08739] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fabb06a5ff5]
[fv-az1947-39:08739] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fabb06bb0da]
[fv-az1947-39:08739] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fabb06a5a55]
[fv-az1947-39:08739] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fabb06a5a6f]
[fv-az1947-39:08739] [ 8] plumed_master(+0x146dd)[0x55e5c274f6dd]
[fv-az1947-39:08739] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fabb022a1ca]
[fv-az1947-39:08739] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fabb022a28b]
[fv-az1947-39:08739] [11] plumed_master(+0x15365)[0x55e5c2750365]
[fv-az1947-39:08739] *** End of error message ***
</pre>
{% endraw %}
