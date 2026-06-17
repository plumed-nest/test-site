**Project ID:** [plumID:19.032]({{ '/' | absolute_url }}eggs/19/032/)  
Stderr for source:  plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action PDB2CONSTANT with label @s95 : argument O1O_lessthan was not set in pdb input
[runnervm7b5n9:11831] *** Process received signal ***
[runnervm7b5n9:11831] Signal: Aborted (6)
[runnervm7b5n9:11831] Signal code:  (-6)
[runnervm7b5n9:11831] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fc67e845330]
[runnervm7b5n9:11831] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fc67e89eb2c]
[runnervm7b5n9:11831] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fc67e84527e]
[runnervm7b5n9:11831] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fc67e8288ff]
[runnervm7b5n9:11831] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fc67eca5ff5]
[runnervm7b5n9:11831] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fc67ecbb0da]
[runnervm7b5n9:11831] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fc67eca5a55]
[runnervm7b5n9:11831] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fc67eca5a6f]
[runnervm7b5n9:11831] [ 8] plumed(+0x146dd)[0x55c319d6d6dd]
[runnervm7b5n9:11831] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fc67e82a1ca]
[runnervm7b5n9:11831] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fc67e82a28b]
[runnervm7b5n9:11831] [11] plumed(+0x15365)[0x55c319d6e365]
[runnervm7b5n9:11831] *** End of error message ***
</pre>
{% endraw %}
