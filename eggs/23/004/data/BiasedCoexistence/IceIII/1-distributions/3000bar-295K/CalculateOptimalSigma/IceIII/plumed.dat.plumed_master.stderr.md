**Project ID:** [plumID:23.004]({{ '/' | absolute_url }}eggs/23/004/)  
Stderr for source:  BiasedCoexistence/IceIII/1-distributions/3000bar-295K/CalculateOptimalSigma/IceIII/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action DUMPGRID with label @78 : keyword ARG is compulsory for this action
[fv-az1436-30:07021] *** Process received signal ***
[fv-az1436-30:07021] Signal: Aborted (6)
[fv-az1436-30:07021] Signal code:  (-6)
[fv-az1436-30:07021] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f4f77045330]
[fv-az1436-30:07021] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f4f7709eb2c]
[fv-az1436-30:07021] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f4f7704527e]
[fv-az1436-30:07021] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f4f770288ff]
[fv-az1436-30:07021] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f4f774a5ff5]
[fv-az1436-30:07021] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f4f774bb0da]
[fv-az1436-30:07021] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f4f774a5a55]
[fv-az1436-30:07021] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f4f774a5a6f]
[fv-az1436-30:07021] [ 8] plumed_master(+0x146dd)[0x561471a726dd]
[fv-az1436-30:07021] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f4f7702a1ca]
[fv-az1436-30:07021] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f4f7702a28b]
[fv-az1436-30:07021] [11] plumed_master(+0x15365)[0x561471a73365]
[fv-az1436-30:07021] *** End of error message ***
</pre>
{% endraw %}
