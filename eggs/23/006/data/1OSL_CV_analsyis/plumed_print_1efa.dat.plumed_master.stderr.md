**Project ID:** [plumID:23.006]({{ '/' | absolute_url }}eggs/23/006/)  
Stderr for source:  1OSL_CV_analsyis/plumed_print_1efa.dat   
Download: [zipped raw stdout](plumed_print_1efa.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_print_1efa.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/GenericMolInfo.cpp:93) PLMD::GenericMolInfo::GenericMolInfo(const PLMD::ActionOptions&)
missing input file 1efa_noTet_99sbws_proc_mod_resID.pdb
[runnervm7b5n9:07267] *** Process received signal ***
[runnervm7b5n9:07267] Signal: Aborted (6)
[runnervm7b5n9:07267] Signal code:  (-6)
[runnervm7b5n9:07267] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f9893245330]
[runnervm7b5n9:07267] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f989329eb2c]
[runnervm7b5n9:07267] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f989324527e]
[runnervm7b5n9:07267] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f98932288ff]
[runnervm7b5n9:07267] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f98936a5ff5]
[runnervm7b5n9:07267] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f98936bb0da]
[runnervm7b5n9:07267] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f98936a5a55]
[runnervm7b5n9:07267] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f98936a5a6f]
[runnervm7b5n9:07267] [ 8] plumed_master(+0x146dd)[0x55d77b5306dd]
[runnervm7b5n9:07267] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f989322a1ca]
[runnervm7b5n9:07267] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f989322a28b]
[runnervm7b5n9:07267] [11] plumed_master(+0x15365)[0x55d77b531365]
[runnervm7b5n9:07267] *** End of error message ***
</pre>
{% endraw %}
