**Project ID:** [plumID:23.001]({{ '/' | absolute_url }}eggs/23/001/)  
Stderr for source:  EnhancedCoexistence/Liq-II/1-BiasedCoexistence/COEX_2000atm/240K/plumed.equil.dat   
Download: [zipped raw stdout](plumed.equil.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.equil.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action ENVIRONMENTSIMILARITY with label @s9 : missing input file ice.pdb
[runnervm7b5n9:06462] *** Process received signal ***
[runnervm7b5n9:06462] Signal: Aborted (6)
[runnervm7b5n9:06462] Signal code:  (-6)
[runnervm7b5n9:06462] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f30fda45330]
[runnervm7b5n9:06462] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f30fda9eb2c]
[runnervm7b5n9:06462] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f30fda4527e]
[runnervm7b5n9:06462] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f30fda288ff]
[runnervm7b5n9:06462] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f30fdea5ff5]
[runnervm7b5n9:06462] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f30fdebb0da]
[runnervm7b5n9:06462] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f30fdea5a55]
[runnervm7b5n9:06462] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f30fdea5a6f]
[runnervm7b5n9:06462] [ 8] plumed_master(+0x146dd)[0x555a873d16dd]
[runnervm7b5n9:06462] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f30fda2a1ca]
[runnervm7b5n9:06462] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f30fda2a28b]
[runnervm7b5n9:06462] [11] plumed_master(+0x15365)[0x555a873d2365]
[runnervm7b5n9:06462] *** End of error message ***
</pre>
{% endraw %}
