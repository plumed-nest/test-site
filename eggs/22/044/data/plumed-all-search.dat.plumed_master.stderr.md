**Project ID:** [plumID:22.044]({{ '/' | absolute_url }}eggs/22/044/)  
Stderr for source:  plumed-all-search.dat   
Download: [zipped raw stdout](plumed-all-search.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed-all-search.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action CONTACT_MATRIX_PROPER with label laq4_mat : problem reading switching function description found the following rogue keywords in switching function input : RATIONAL
[fv-az1718-879:07032] *** Process received signal ***
[fv-az1718-879:07032] Signal: Aborted (6)
[fv-az1718-879:07032] Signal code:  (-6)
[fv-az1718-879:07032] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f01ede45330]
[fv-az1718-879:07032] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f01ede9eb2c]
[fv-az1718-879:07032] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f01ede4527e]
[fv-az1718-879:07032] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f01ede288ff]
[fv-az1718-879:07032] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f01ee2a5ff5]
[fv-az1718-879:07032] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f01ee2bb0da]
[fv-az1718-879:07032] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f01ee2a5a55]
[fv-az1718-879:07032] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f01ee2a5a6f]
[fv-az1718-879:07032] [ 8] plumed_master(+0x146dd)[0x55c5a5b5a6dd]
[fv-az1718-879:07032] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f01ede2a1ca]
[fv-az1718-879:07032] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f01ede2a28b]
[fv-az1718-879:07032] [11] plumed_master(+0x15365)[0x55c5a5b5b365]
[fv-az1718-879:07032] *** End of error message ***
</pre>
{% endraw %}
