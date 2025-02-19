**Project ID:** [plumID:23.026]({{ '/' | absolute_url }}eggs/23/026/)  
Stderr for source:  plumed_model_pulling.dat   
Download: [zipped raw stdout](plumed_model_pulling.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_model_pulling.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "PYTHONCV" is not known.
[fv-az1945-156:07078] *** Process received signal ***
[fv-az1945-156:07078] Signal: Aborted (6)
[fv-az1945-156:07078] Signal code:  (-6)
[fv-az1945-156:07078] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f7fc3245330]
[fv-az1945-156:07078] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f7fc329eb2c]
[fv-az1945-156:07078] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f7fc324527e]
[fv-az1945-156:07078] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f7fc32288ff]
[fv-az1945-156:07078] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f7fc36a5ff5]
[fv-az1945-156:07078] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f7fc36bb0da]
[fv-az1945-156:07078] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f7fc36a5a55]
[fv-az1945-156:07078] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f7fc36a5a6f]
[fv-az1945-156:07078] [ 8] plumed_master(+0x146dd)[0x5643e28876dd]
[fv-az1945-156:07078] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f7fc322a1ca]
[fv-az1945-156:07078] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f7fc322a28b]
[fv-az1945-156:07078] [11] plumed_master(+0x15365)[0x5643e2888365]
[fv-az1945-156:07078] *** End of error message ***
</pre>
{% endraw %}
