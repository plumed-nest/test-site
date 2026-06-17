**Project ID:** [plumID:22.044]({{ '/' | absolute_url }}eggs/22/044/)  
Stderr for source:  plumed-all-search.dat   
Download: [zipped raw stdout](plumed-all-search.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed-all-search.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action CONTACT_MATRIX_PROPER with label laq4_mat : problem reading switching function description found the following rogue keywords in switching function input : RATIONAL
[runnervm7b5n9:07048] *** Process received signal ***
[runnervm7b5n9:07048] Signal: Aborted (6)
[runnervm7b5n9:07048] Signal code:  (-6)
[runnervm7b5n9:07048] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f205c645330]
[runnervm7b5n9:07048] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f205c69eb2c]
[runnervm7b5n9:07048] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f205c64527e]
[runnervm7b5n9:07048] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f205c6288ff]
[runnervm7b5n9:07048] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f205caa5ff5]
[runnervm7b5n9:07048] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f205cabb0da]
[runnervm7b5n9:07048] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f205caa5a55]
[runnervm7b5n9:07048] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f205caa5a6f]
[runnervm7b5n9:07048] [ 8] plumed_master(+0x146dd)[0x5638c82f86dd]
[runnervm7b5n9:07048] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f205c62a1ca]
[runnervm7b5n9:07048] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f205c62a28b]
[runnervm7b5n9:07048] [11] plumed_master(+0x15365)[0x5638c82f9365]
[runnervm7b5n9:07048] *** End of error message ***
</pre>
{% endraw %}
