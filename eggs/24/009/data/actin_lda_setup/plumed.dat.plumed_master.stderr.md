**Project ID:** [plumID:24.009]({{ '/' | absolute_url }}eggs/24/009/)  
Stderr for source:  actin_lda_setup/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "LDA_PROJ" is not known.
[fv-az1947-39:07383] *** Process received signal ***
[fv-az1947-39:07383] Signal: Aborted (6)
[fv-az1947-39:07383] Signal code:  (-6)
[fv-az1947-39:07383] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f9854045330]
[fv-az1947-39:07383] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f985409eb2c]
[fv-az1947-39:07383] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f985404527e]
[fv-az1947-39:07383] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f98540288ff]
[fv-az1947-39:07383] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f98544a5ff5]
[fv-az1947-39:07383] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f98544bb0da]
[fv-az1947-39:07383] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f98544a5a55]
[fv-az1947-39:07383] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f98544a5a6f]
[fv-az1947-39:07383] [ 8] plumed_master(+0x146dd)[0x559fc77636dd]
[fv-az1947-39:07383] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f985402a1ca]
[fv-az1947-39:07383] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f985402a28b]
[fv-az1947-39:07383] [11] plumed_master(+0x15365)[0x559fc7764365]
[fv-az1947-39:07383] *** End of error message ***
</pre>
{% endraw %}
