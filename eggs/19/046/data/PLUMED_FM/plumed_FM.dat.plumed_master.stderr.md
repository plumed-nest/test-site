**Project ID:** [plumID:19.046]({{ '/' | absolute_url }}eggs/19/046/)  
Stderr for source:  PLUMED_FM/plumed_FM.dat   
Download: [zipped raw stdout](plumed_FM.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_FM.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "FPS" is not known.
[fv-az2027-338:10703] *** Process received signal ***
[fv-az2027-338:10703] Signal: Aborted (6)
[fv-az2027-338:10703] Signal code:  (-6)
[fv-az2027-338:10703] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fc4c3045330]
[fv-az2027-338:10703] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fc4c309eb2c]
[fv-az2027-338:10703] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fc4c304527e]
[fv-az2027-338:10703] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fc4c30288ff]
[fv-az2027-338:10703] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fc4c34a5ff5]
[fv-az2027-338:10703] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fc4c34bb0da]
[fv-az2027-338:10703] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fc4c34a5a55]
[fv-az2027-338:10703] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fc4c34a5a6f]
[fv-az2027-338:10703] [ 8] plumed_master(+0x146dd)[0x5610ab2df6dd]
[fv-az2027-338:10703] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fc4c302a1ca]
[fv-az2027-338:10703] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fc4c302a28b]
[fv-az2027-338:10703] [11] plumed_master(+0x15365)[0x5610ab2e0365]
[fv-az2027-338:10703] *** End of error message ***
</pre>
{% endraw %}
