**Project ID:** [plumID:23.001]({{ '/' | absolute_url }}eggs/23/001/)  
Stderr for source:  EnhancedCoexistence/Liq-II/1-BiasedCoexistence/COEX_2000atm/240K/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action ENVIRONMENTSIMILARITY with label @s10 : missing input file ice.pdb
[fv-az1947-39:07836] *** Process received signal ***
[fv-az1947-39:07836] Signal: Aborted (6)
[fv-az1947-39:07836] Signal code:  (-6)
[fv-az1947-39:07836] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f269ca45330]
[fv-az1947-39:07836] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f269ca9eb2c]
[fv-az1947-39:07836] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f269ca4527e]
[fv-az1947-39:07836] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f269ca288ff]
[fv-az1947-39:07836] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f269cea5ff5]
[fv-az1947-39:07836] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f269cebb0da]
[fv-az1947-39:07836] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f269cea5a55]
[fv-az1947-39:07836] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f269cea5a6f]
[fv-az1947-39:07836] [ 8] plumed(+0x146dd)[0x560134ebd6dd]
[fv-az1947-39:07836] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f269ca2a1ca]
[fv-az1947-39:07836] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f269ca2a28b]
[fv-az1947-39:07836] [11] plumed(+0x15365)[0x560134ebe365]
[fv-az1947-39:07836] *** End of error message ***
</pre>
{% endraw %}
