**Project ID:** [plumID:21.018]({{ '/' | absolute_url }}eggs/21/018/)  
Stderr for source:  plumed_reweight/reweight_rho_hb.dat   
Download: [zipped raw stdout](reweight_rho_hb.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](reweight_rho_hb.dat.plumed_master.stderr.txt.zip) 
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
ERROR in input to action DUMPGRID with label @34 : keyword ARG is compulsory for this action
[fv-az1945-156:12661] *** Process received signal ***
[fv-az1945-156:12661] Signal: Aborted (6)
[fv-az1945-156:12661] Signal code:  (-6)
[fv-az1945-156:12661] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fbfdae45330]
[fv-az1945-156:12661] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fbfdae9eb2c]
[fv-az1945-156:12661] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fbfdae4527e]
[fv-az1945-156:12661] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fbfdae288ff]
[fv-az1945-156:12661] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fbfdb2a5ff5]
[fv-az1945-156:12661] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fbfdb2bb0da]
[fv-az1945-156:12661] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fbfdb2a5a55]
[fv-az1945-156:12661] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fbfdb2a5a6f]
[fv-az1945-156:12661] [ 8] plumed_master(+0x146dd)[0x55ce4a2f26dd]
[fv-az1945-156:12661] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fbfdae2a1ca]
[fv-az1945-156:12661] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fbfdae2a28b]
[fv-az1945-156:12661] [11] plumed_master(+0x15365)[0x55ce4a2f3365]
[fv-az1945-156:12661] *** End of error message ***
</pre>
{% endraw %}
