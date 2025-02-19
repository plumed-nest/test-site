**Project ID:** [plumID:21.013]({{ '/' | absolute_url }}eggs/21/013/)  
Stderr for source:  ch4-diss/ni111-symm/plumed.inp   
Download: [zipped raw stdout](plumed.inp.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.inp.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
Assembler messages:
Fatal error: can't create plumed_mklib.84N4Wl/../../data/ReweightGeomFES.o: No such file or directory
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:1499) void PLMD::PlumedMain::load(const std::string&)
An error happened while executing command env PLUMED_ROOT='/home/runner/opt/lib/plumed_master' PLUMED_VERSION='2.11.0-dev' PLUMED_HTMLDIR='/home/runner/opt/share/doc/plumed_master' PLUMED_INCLUDEDIR='/home/runner/opt/include' PLUMED_PROGRAM_NAME='plumed_master' PLUMED_IS_INSTALLED='yes' "/home/runner/opt/lib/plumed_master"/scripts/mklib.sh -n -o ./../../data/ReweightGeomFES.2.11.0-dev.so ../../data/ReweightGeomFES.cpp

[fv-az1947-39:11817] *** Process received signal ***
[fv-az1947-39:11817] Signal: Aborted (6)
[fv-az1947-39:11817] Signal code:  (-6)
[fv-az1947-39:11817] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f505b245330]
[fv-az1947-39:11817] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f505b29eb2c]
[fv-az1947-39:11817] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f505b24527e]
[fv-az1947-39:11817] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f505b2288ff]
[fv-az1947-39:11817] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f505b6a5ff5]
[fv-az1947-39:11817] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f505b6bb0da]
[fv-az1947-39:11817] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f505b6a5a55]
[fv-az1947-39:11817] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f505b6a5a6f]
[fv-az1947-39:11817] [ 8] plumed_master(+0x146dd)[0x555fa31196dd]
[fv-az1947-39:11817] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f505b22a1ca]
[fv-az1947-39:11817] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f505b22a28b]
[fv-az1947-39:11817] [11] plumed_master(+0x15365)[0x555fa311a365]
[fv-az1947-39:11817] *** End of error message ***
</pre>
{% endraw %}
