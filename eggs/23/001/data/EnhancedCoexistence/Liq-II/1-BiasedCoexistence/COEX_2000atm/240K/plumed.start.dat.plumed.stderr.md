**Project ID:** [plumID:23.001]({{ '/' | absolute_url }}eggs/23/001/)  
Stderr for source:  EnhancedCoexistence/Liq-II/1-BiasedCoexistence/COEX_2000atm/240K/plumed.start.dat   
Download: [zipped raw stdout](plumed.start.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.start.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action ENVIRONMENTSIMILARITY with label @s9 : missing input file ice.pdb
[runnervm7b5n9:06551] *** Process received signal ***
[runnervm7b5n9:06551] Signal: Aborted (6)
[runnervm7b5n9:06551] Signal code:  (-6)
[runnervm7b5n9:06551] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fb8f1245330]
[runnervm7b5n9:06551] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fb8f129eb2c]
[runnervm7b5n9:06551] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fb8f124527e]
[runnervm7b5n9:06551] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fb8f12288ff]
[runnervm7b5n9:06551] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fb8f16a5ff5]
[runnervm7b5n9:06551] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fb8f16bb0da]
[runnervm7b5n9:06551] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fb8f16a5a55]
[runnervm7b5n9:06551] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fb8f16a5a6f]
[runnervm7b5n9:06551] [ 8] plumed(+0x146dd)[0x55709fd3a6dd]
[runnervm7b5n9:06551] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fb8f122a1ca]
[runnervm7b5n9:06551] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fb8f122a28b]
[runnervm7b5n9:06551] [11] plumed(+0x15365)[0x55709fd3b365]
[runnervm7b5n9:06551] *** End of error message ***
</pre>
{% endraw %}
