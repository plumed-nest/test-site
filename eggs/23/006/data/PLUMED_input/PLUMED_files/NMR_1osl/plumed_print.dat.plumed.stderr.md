**Project ID:** [plumID:23.006]({{ '/' | absolute_url }}eggs/23/006/)  
Stderr for source:  PLUMED_input/PLUMED_files/NMR_1osl/plumed_print.dat   
Download: [zipped raw stdout](plumed_print.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_print.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/GenericMolInfo.cpp:89) PLMD::GenericMolInfo::GenericMolInfo(const PLMD::ActionOptions&)
missing input file 1osl_C52V_GMX_new_numbering.pdb
[fv-az659-568:39460] *** Process received signal ***
[fv-az659-568:39460] Signal: Aborted (6)
[fv-az659-568:39460] Signal code:  (-6)
[fv-az659-568:39460] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f8359a42520]
[fv-az659-568:39460] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f8359a969fc]
[fv-az659-568:39460] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f8359a42476]
[fv-az659-568:39460] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f8359a287f3]
[fv-az659-568:39460] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f8359ea2b9e]
[fv-az659-568:39460] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f8359eae20c]
[fv-az659-568:39460] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f8359eae277]
[fv-az659-568:39460] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f8359eae52b]
[fv-az659-568:39460] [ 8] plumed(+0x12f48)[0x55966c33af48]
[fv-az659-568:39460] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f8359a29d90]
[fv-az659-568:39460] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f8359a29e40]
[fv-az659-568:39460] [11] plumed(+0x131e5)[0x55966c33b1e5]
[fv-az659-568:39460] *** End of error message ***
</pre>
{% endraw %}
