**Project ID:** [plumID:19.027]({{ '/' | absolute_url }}eggs/19/027/)  
Stderr for source:  MulticanonicalSimulations/References/Temp400K/Distribution/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
WARNING: IFile closed in the middle of reading. seems strange!
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action DUMPGRID with label @28 : keyword ARG is compulsory for this action
[fv-az1718-879:12099] *** Process received signal ***
[fv-az1718-879:12099] Signal: Aborted (6)
[fv-az1718-879:12099] Signal code:  (-6)
[fv-az1718-879:12099] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fccaa245330]
[fv-az1718-879:12099] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fccaa29eb2c]
[fv-az1718-879:12099] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fccaa24527e]
[fv-az1718-879:12099] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fccaa2288ff]
[fv-az1718-879:12099] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fccaa6a5ff5]
[fv-az1718-879:12099] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fccaa6bb0da]
[fv-az1718-879:12099] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fccaa6a5a55]
[fv-az1718-879:12099] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fccaa6a5a6f]
[fv-az1718-879:12099] [ 8] plumed_master(+0x146dd)[0x559039df86dd]
[fv-az1718-879:12099] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fccaa22a1ca]
[fv-az1718-879:12099] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fccaa22a28b]
[fv-az1718-879:12099] [11] plumed_master(+0x15365)[0x559039df9365]
[fv-az1718-879:12099] *** End of error message ***
</pre>
{% endraw %}
