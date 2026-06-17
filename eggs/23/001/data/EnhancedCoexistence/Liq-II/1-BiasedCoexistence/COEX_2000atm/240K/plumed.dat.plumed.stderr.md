**Project ID:** [plumID:23.001]({{ '/' | absolute_url }}eggs/23/001/)  
Stderr for source:  EnhancedCoexistence/Liq-II/1-BiasedCoexistence/COEX_2000atm/240K/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action ENVIRONMENTSIMILARITY with label @s10 : missing input file ice.pdb
[runnervm7b5n9:06394] *** Process received signal ***
[runnervm7b5n9:06394] Signal: Aborted (6)
[runnervm7b5n9:06394] Signal code:  (-6)
[runnervm7b5n9:06394] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f3765845330]
[runnervm7b5n9:06394] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f376589eb2c]
[runnervm7b5n9:06394] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f376584527e]
[runnervm7b5n9:06394] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f37658288ff]
[runnervm7b5n9:06394] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f3765ca5ff5]
[runnervm7b5n9:06394] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f3765cbb0da]
[runnervm7b5n9:06394] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f3765ca5a55]
[runnervm7b5n9:06394] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f3765ca5a6f]
[runnervm7b5n9:06394] [ 8] plumed(+0x146dd)[0x5628e3ce66dd]
[runnervm7b5n9:06394] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f376582a1ca]
[runnervm7b5n9:06394] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f376582a28b]
[runnervm7b5n9:06394] [11] plumed(+0x15365)[0x5628e3ce7365]
[runnervm7b5n9:06394] *** End of error message ***
</pre>
{% endraw %}
