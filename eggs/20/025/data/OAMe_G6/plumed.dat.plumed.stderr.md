**Project ID:** [plumID:20.025]({{ '/' | absolute_url }}eggs/20/025/)  
Stderr for source:  OAMe_G6/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::add_buffer_to<std::bad_alloc>'
what():  std::bad_alloc
[fv-az2027-338:10466] *** Process received signal ***
[fv-az2027-338:10466] Signal: Aborted (6)
[fv-az2027-338:10466] Signal code:  (-6)
[fv-az2027-338:10466] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fa539c45330]
[fv-az2027-338:10466] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fa539c9eb2c]
[fv-az2027-338:10466] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fa539c4527e]
[fv-az2027-338:10466] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fa539c288ff]
[fv-az2027-338:10466] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fa53a0a5ff5]
[fv-az2027-338:10466] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fa53a0bb0da]
[fv-az2027-338:10466] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fa53a0a5a55]
[fv-az2027-338:10466] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fa53a0a5a6f]
[fv-az2027-338:10466] [ 8] plumed(+0x146dd)[0x558d520936dd]
[fv-az2027-338:10466] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fa539c2a1ca]
[fv-az2027-338:10466] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fa539c2a28b]
[fv-az2027-338:10466] [11] plumed(+0x15365)[0x558d52094365]
[fv-az2027-338:10466] *** End of error message ***
</pre>
{% endraw %}
