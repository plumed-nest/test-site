**Project ID:** [plumID:23.004]({{ '/' | absolute_url }}eggs/23/004/)  
Stderr for source:  BiasedCoexistence/IceIII/1-distributions/3000bar-295K/CalculateOptimalSigma/IceIII/plumed-base.dat   
Download: [zipped raw stdout](plumed-base.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed-base.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action DUMPGRID with label @78 : keyword ARG is compulsory for this action
[fv-az1436-30:06977] *** Process received signal ***
[fv-az1436-30:06977] Signal: Aborted (6)
[fv-az1436-30:06977] Signal code:  (-6)
[fv-az1436-30:06977] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f3f72045330]
[fv-az1436-30:06977] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f3f7209eb2c]
[fv-az1436-30:06977] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f3f7204527e]
[fv-az1436-30:06977] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f3f720288ff]
[fv-az1436-30:06977] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f3f724a5ff5]
[fv-az1436-30:06977] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f3f724bb0da]
[fv-az1436-30:06977] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f3f724a5a55]
[fv-az1436-30:06977] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f3f724a5a6f]
[fv-az1436-30:06977] [ 8] plumed_master(+0x146dd)[0x564d316d26dd]
[fv-az1436-30:06977] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f3f7202a1ca]
[fv-az1436-30:06977] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f3f7202a28b]
[fv-az1436-30:06977] [11] plumed_master(+0x15365)[0x564d316d3365]
[fv-az1436-30:06977] *** End of error message ***
</pre>
{% endraw %}
