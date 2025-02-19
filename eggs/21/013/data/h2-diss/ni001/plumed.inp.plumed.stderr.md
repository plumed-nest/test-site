**Project ID:** [plumID:21.013]({{ '/' | absolute_url }}eggs/21/013/)  
Stderr for source:  h2-diss/ni001/plumed.inp   
Download: [zipped raw stdout](plumed.inp.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.inp.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
Assembler messages:
Fatal error: can't create plumed_mklib.O70Xvx/../../data/ReweightGeomFES.o: No such file or directory
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:1499) void PLMD::PlumedMain::load(const std::string&)
An error happened while executing command env PLUMED_ROOT='/home/runner/opt/lib/plumed' PLUMED_VERSION='2.10b' PLUMED_HTMLDIR='/home/runner/opt/share/doc/plumed' PLUMED_INCLUDEDIR='/home/runner/opt/include' PLUMED_PROGRAM_NAME='plumed' PLUMED_IS_INSTALLED='yes' "/home/runner/opt/lib/plumed"/scripts/mklib.sh -n -o ./../../data/ReweightGeomFES.2.10b.so ../../data/ReweightGeomFES.cpp

[fv-az1947-39:11147] *** Process received signal ***
[fv-az1947-39:11147] Signal: Aborted (6)
[fv-az1947-39:11147] Signal code:  (-6)
[fv-az1947-39:11147] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f9c57845330]
[fv-az1947-39:11147] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f9c5789eb2c]
[fv-az1947-39:11147] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f9c5784527e]
[fv-az1947-39:11147] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f9c578288ff]
[fv-az1947-39:11147] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f9c57ca5ff5]
[fv-az1947-39:11147] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f9c57cbb0da]
[fv-az1947-39:11147] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f9c57ca5a55]
[fv-az1947-39:11147] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f9c57ca5a6f]
[fv-az1947-39:11147] [ 8] plumed(+0x146dd)[0x558da38516dd]
[fv-az1947-39:11147] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f9c5782a1ca]
[fv-az1947-39:11147] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f9c5782a28b]
[fv-az1947-39:11147] [11] plumed(+0x15365)[0x558da3852365]
[fv-az1947-39:11147] *** End of error message ***
</pre>
{% endraw %}
