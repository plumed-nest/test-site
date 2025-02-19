**Project ID:** [plumID:23.016]({{ '/' | absolute_url }}eggs/23/016/)  
Stderr for source:  plumed_reweight_2D_microsw_adr_bin.dat   
Download: [zipped raw stdout](plumed_reweight_2D_microsw_adr_bin.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_reweight_2D_microsw_adr_bin.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action DUMPGRID with label @90 : keyword ARG is compulsory for this action
[fv-az1326-415:08714] *** Process received signal ***
[fv-az1326-415:08714] Signal: Aborted (6)
[fv-az1326-415:08714] Signal code:  (-6)
[fv-az1326-415:08714] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f66b8445330]
[fv-az1326-415:08714] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f66b849eb2c]
[fv-az1326-415:08714] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f66b844527e]
[fv-az1326-415:08714] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f66b84288ff]
[fv-az1326-415:08714] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f66b88a5ff5]
[fv-az1326-415:08714] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f66b88bb0da]
[fv-az1326-415:08714] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f66b88a5a55]
[fv-az1326-415:08714] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f66b88a5a6f]
[fv-az1326-415:08714] [ 8] plumed_master(+0x146dd)[0x560c6e80f6dd]
[fv-az1326-415:08714] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f66b842a1ca]
[fv-az1326-415:08714] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f66b842a28b]
[fv-az1326-415:08714] [11] plumed_master(+0x15365)[0x560c6e810365]
[fv-az1326-415:08714] *** End of error message ***
</pre>
{% endraw %}
