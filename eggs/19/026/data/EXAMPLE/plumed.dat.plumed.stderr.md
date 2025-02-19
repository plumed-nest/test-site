**Project ID:** [plumID:19.026]({{ '/' | absolute_url }}eggs/19/026/)  
Stderr for source:  EXAMPLE/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "HBOND_COORD" is not known.
[fv-az1770-999:12402] *** Process received signal ***
[fv-az1770-999:12402] Signal: Aborted (6)
[fv-az1770-999:12402] Signal code:  (-6)
[fv-az1770-999:12402] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f6ffa845330]
[fv-az1770-999:12402] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f6ffa89eb2c]
[fv-az1770-999:12402] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f6ffa84527e]
[fv-az1770-999:12402] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f6ffa8288ff]
[fv-az1770-999:12402] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f6ffaca5ff5]
[fv-az1770-999:12402] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f6ffacbb0da]
[fv-az1770-999:12402] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f6ffaca5a55]
[fv-az1770-999:12402] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f6ffaca5a6f]
[fv-az1770-999:12402] [ 8] plumed(+0x146dd)[0x555e370be6dd]
[fv-az1770-999:12402] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f6ffa82a1ca]
[fv-az1770-999:12402] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f6ffa82a28b]
[fv-az1770-999:12402] [11] plumed(+0x15365)[0x555e370bf365]
[fv-az1770-999:12402] *** End of error message ***
</pre>
{% endraw %}
