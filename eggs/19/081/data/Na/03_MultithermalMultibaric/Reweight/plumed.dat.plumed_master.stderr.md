**Project ID:** [plumID:19.081]({{ '/' | absolute_url }}eggs/19/081/)  
Stderr for source:  Na/03_MultithermalMultibaric/Reweight/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
WARNING: IFile closed in the middle of reading. seems strange!
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action DUMPGRID with label @40 : keyword ARG is compulsory for this action
[fv-az1770-999:10727] *** Process received signal ***
[fv-az1770-999:10727] Signal: Aborted (6)
[fv-az1770-999:10727] Signal code:  (-6)
[fv-az1770-999:10727] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f2e68845330]
[fv-az1770-999:10727] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f2e6889eb2c]
[fv-az1770-999:10727] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f2e6884527e]
[fv-az1770-999:10727] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f2e688288ff]
[fv-az1770-999:10727] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f2e68ca5ff5]
[fv-az1770-999:10727] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f2e68cbb0da]
[fv-az1770-999:10727] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f2e68ca5a55]
[fv-az1770-999:10727] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f2e68ca5a6f]
[fv-az1770-999:10727] [ 8] plumed_master(+0x146dd)[0x55c05479d6dd]
[fv-az1770-999:10727] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f2e6882a1ca]
[fv-az1770-999:10727] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f2e6882a28b]
[fv-az1770-999:10727] [11] plumed_master(+0x15365)[0x55c05479e365]
[fv-az1770-999:10727] *** End of error message ***
</pre>
{% endraw %}
