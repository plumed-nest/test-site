**Project ID:** [plumID:23.006]({{ '/' | absolute_url }}eggs/23/006/)  
Stderr for source:  PLUMED_input/PLUMED_files/NMR_1osl/plumed_print.dat   
Download: [zipped raw stdout](plumed_print.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_print.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/GenericMolInfo.cpp:89) PLMD::GenericMolInfo::GenericMolInfo(const PLMD::ActionOptions&)
missing input file 1osl_C52V_GMX_new_numbering.pdb
[fv-az841-65:69849] *** Process received signal ***
[fv-az841-65:69849] Signal: Aborted (6)
[fv-az841-65:69849] Signal code:  (-6)
[fv-az841-65:69849] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f2337e42520]
[fv-az841-65:69849] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f2337e969fc]
[fv-az841-65:69849] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f2337e42476]
[fv-az841-65:69849] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f2337e287f3]
[fv-az841-65:69849] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f23382a2b9e]
[fv-az841-65:69849] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f23382ae20c]
[fv-az841-65:69849] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f23382ae277]
[fv-az841-65:69849] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f23382ae52b]
[fv-az841-65:69849] [ 8] plumed_master(+0x14274)[0x557770837274]
[fv-az841-65:69849] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f2337e29d90]
[fv-az841-65:69849] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f2337e29e40]
[fv-az841-65:69849] [11] plumed_master(+0x14ed5)[0x557770837ed5]
[fv-az841-65:69849] *** End of error message ***
</pre>
{% endraw %}
