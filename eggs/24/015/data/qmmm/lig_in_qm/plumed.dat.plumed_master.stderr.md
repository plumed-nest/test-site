**Project ID:** [plumID:24.015]({{ '/' | absolute_url }}eggs/24/015/)  
Stderr for source:  qmmm/lig_in_qm/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "PATHCV" is not known.
[fv-az2027-338:05837] *** Process received signal ***
[fv-az2027-338:05837] Signal: Aborted (6)
[fv-az2027-338:05837] Signal code:  (-6)
[fv-az2027-338:05837] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7ff412a45330]
[fv-az2027-338:05837] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7ff412a9eb2c]
[fv-az2027-338:05837] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7ff412a4527e]
[fv-az2027-338:05837] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7ff412a288ff]
[fv-az2027-338:05837] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7ff412ea5ff5]
[fv-az2027-338:05837] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7ff412ebb0da]
[fv-az2027-338:05837] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7ff412ea5a55]
[fv-az2027-338:05837] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7ff412ea5a6f]
[fv-az2027-338:05837] [ 8] plumed_master(+0x146dd)[0x55be904bb6dd]
[fv-az2027-338:05837] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7ff412a2a1ca]
[fv-az2027-338:05837] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7ff412a2a28b]
[fv-az2027-338:05837] [11] plumed_master(+0x15365)[0x55be904bc365]
[fv-az2027-338:05837] *** End of error message ***
</pre>
{% endraw %}
