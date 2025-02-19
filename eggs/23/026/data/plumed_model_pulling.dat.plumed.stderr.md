**Project ID:** [plumID:23.026]({{ '/' | absolute_url }}eggs/23/026/)  
Stderr for source:  plumed_model_pulling.dat   
Download: [zipped raw stdout](plumed_model_pulling.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_model_pulling.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "PYTHONCV" is not known.
[fv-az1945-156:07062] *** Process received signal ***
[fv-az1945-156:07062] Signal: Aborted (6)
[fv-az1945-156:07062] Signal code:  (-6)
[fv-az1945-156:07062] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fe6c0c45330]
[fv-az1945-156:07062] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fe6c0c9eb2c]
[fv-az1945-156:07062] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fe6c0c4527e]
[fv-az1945-156:07062] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fe6c0c288ff]
[fv-az1945-156:07062] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fe6c10a5ff5]
[fv-az1945-156:07062] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fe6c10bb0da]
[fv-az1945-156:07062] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fe6c10a5a55]
[fv-az1945-156:07062] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fe6c10a5a6f]
[fv-az1945-156:07062] [ 8] plumed(+0x146dd)[0x56306dcbf6dd]
[fv-az1945-156:07062] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fe6c0c2a1ca]
[fv-az1945-156:07062] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fe6c0c2a28b]
[fv-az1945-156:07062] [11] plumed(+0x15365)[0x56306dcc0365]
[fv-az1945-156:07062] *** End of error message ***
</pre>
{% endraw %}
