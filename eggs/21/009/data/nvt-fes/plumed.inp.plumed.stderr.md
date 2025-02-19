**Project ID:** [plumID:21.009]({{ '/' | absolute_url }}eggs/21/009/)  
Stderr for source:  nvt-fes/plumed.inp   
Download: [zipped raw stdout](plumed.inp.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.inp.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
Assembler messages:
Fatal error: can't create plumed_mklib.at5PlJ/../codes/ReweightGeomFES.o: No such file or directory
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:1499) void PLMD::PlumedMain::load(const std::string&)
An error happened while executing command env PLUMED_ROOT='/home/runner/opt/lib/plumed' PLUMED_VERSION='2.10b' PLUMED_HTMLDIR='/home/runner/opt/share/doc/plumed' PLUMED_INCLUDEDIR='/home/runner/opt/include' PLUMED_PROGRAM_NAME='plumed' PLUMED_IS_INSTALLED='yes' "/home/runner/opt/lib/plumed"/scripts/mklib.sh -n -o ./../codes/ReweightGeomFES.2.10b.so ../codes/ReweightGeomFES.cpp

[fv-az1718-879:09900] *** Process received signal ***
[fv-az1718-879:09900] Signal: Aborted (6)
[fv-az1718-879:09900] Signal code:  (-6)
[fv-az1718-879:09900] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f75e7245330]
[fv-az1718-879:09900] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f75e729eb2c]
[fv-az1718-879:09900] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f75e724527e]
[fv-az1718-879:09900] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f75e72288ff]
[fv-az1718-879:09900] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f75e76a5ff5]
[fv-az1718-879:09900] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f75e76bb0da]
[fv-az1718-879:09900] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f75e76a5a55]
[fv-az1718-879:09900] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f75e76a5a6f]
[fv-az1718-879:09900] [ 8] plumed(+0x146dd)[0x558af11186dd]
[fv-az1718-879:09900] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f75e722a1ca]
[fv-az1718-879:09900] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f75e722a28b]
[fv-az1718-879:09900] [11] plumed(+0x15365)[0x558af1119365]
[fv-az1718-879:09900] *** End of error message ***
</pre>
{% endraw %}
