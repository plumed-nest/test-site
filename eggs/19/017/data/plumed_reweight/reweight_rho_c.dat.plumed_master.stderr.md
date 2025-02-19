**Project ID:** [plumID:19.017]({{ '/' | absolute_url }}eggs/19/017/)  
Stderr for source:  plumed_reweight/reweight_rho_c.dat   
Download: [zipped raw stdout](reweight_rho_c.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](reweight_rho_c.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
WARNING: IFile closed in the middle of reading. seems strange!
WARNING: IFile closed in the middle of reading. seems strange!
WARNING: IFile closed in the middle of reading. seems strange!
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action DUMPGRID with label @17 : keyword ARG is compulsory for this action
[fv-az1672-644:08928] *** Process received signal ***
[fv-az1672-644:08928] Signal: Aborted (6)
[fv-az1672-644:08928] Signal code:  (-6)
[fv-az1672-644:08928] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f832be45330]
[fv-az1672-644:08928] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f832be9eb2c]
[fv-az1672-644:08928] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f832be4527e]
[fv-az1672-644:08928] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f832be288ff]
[fv-az1672-644:08928] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f832c2a5ff5]
[fv-az1672-644:08928] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f832c2bb0da]
[fv-az1672-644:08928] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f832c2a5a55]
[fv-az1672-644:08928] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f832c2a5a6f]
[fv-az1672-644:08928] [ 8] plumed_master(+0x146dd)[0x5596bf6ab6dd]
[fv-az1672-644:08928] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f832be2a1ca]
[fv-az1672-644:08928] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f832be2a28b]
[fv-az1672-644:08928] [11] plumed_master(+0x15365)[0x5596bf6ac365]
[fv-az1672-644:08928] *** End of error message ***
</pre>
{% endraw %}
