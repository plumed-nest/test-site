**Project ID:** [plumID:22.025]({{ '/' | absolute_url }}eggs/22/025/)  
Stderr for source:  t0.700/p0.16222-fes/plumed.inp   
Download: [zipped raw stdout](plumed.inp.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.inp.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
Assembler messages:
Fatal error: can't create plumed_mklib.dSIchL/../../code/ReweightGeomFES.o: No such file or directory
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:1499) void PLMD::PlumedMain::load(const std::string&)
An error happened while executing command env PLUMED_ROOT='/home/runner/opt/lib/plumed' PLUMED_VERSION='2.10b' PLUMED_HTMLDIR='/home/runner/opt/share/doc/plumed' PLUMED_INCLUDEDIR='/home/runner/opt/include' PLUMED_PROGRAM_NAME='plumed' PLUMED_IS_INSTALLED='yes' "/home/runner/opt/lib/plumed"/scripts/mklib.sh -n -o ./../../code/ReweightGeomFES.2.10b.so ../../code/ReweightGeomFES.cpp

[fv-az1945-156:08750] *** Process received signal ***
[fv-az1945-156:08750] Signal: Aborted (6)
[fv-az1945-156:08750] Signal code:  (-6)
[fv-az1945-156:08750] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f49b7645330]
[fv-az1945-156:08750] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f49b769eb2c]
[fv-az1945-156:08750] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f49b764527e]
[fv-az1945-156:08750] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f49b76288ff]
[fv-az1945-156:08750] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f49b7aa5ff5]
[fv-az1945-156:08750] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f49b7abb0da]
[fv-az1945-156:08750] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f49b7aa5a55]
[fv-az1945-156:08750] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f49b7aa5a6f]
[fv-az1945-156:08750] [ 8] plumed(+0x146dd)[0x55fd2aa186dd]
[fv-az1945-156:08750] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f49b762a1ca]
[fv-az1945-156:08750] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f49b762a28b]
[fv-az1945-156:08750] [11] plumed(+0x15365)[0x55fd2aa19365]
[fv-az1945-156:08750] *** End of error message ***
</pre>
{% endraw %}
