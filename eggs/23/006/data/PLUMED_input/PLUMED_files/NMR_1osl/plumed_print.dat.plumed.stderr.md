**Project ID:** [plumID:23.006]({{ '/' | absolute_url }}eggs/23/006/)  
Stderr for source:  PLUMED_input/PLUMED_files/NMR_1osl/plumed_print.dat   
Download: [zipped raw stdout](plumed_print.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_print.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/GenericMolInfo.cpp:93) PLMD::GenericMolInfo::GenericMolInfo(const PLMD::ActionOptions&)
missing input file 1osl_C52V_GMX_new_numbering.pdb
[runnervm7b5n9:07354] *** Process received signal ***
[runnervm7b5n9:07354] Signal: Aborted (6)
[runnervm7b5n9:07354] Signal code:  (-6)
[runnervm7b5n9:07354] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f208d245330]
[runnervm7b5n9:07354] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f208d29eb2c]
[runnervm7b5n9:07354] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f208d24527e]
[runnervm7b5n9:07354] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f208d2288ff]
[runnervm7b5n9:07354] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f208d6a5ff5]
[runnervm7b5n9:07354] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f208d6bb0da]
[runnervm7b5n9:07354] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f208d6a5a55]
[runnervm7b5n9:07354] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f208d6a5a6f]
[runnervm7b5n9:07354] [ 8] plumed(+0x146dd)[0x563751afe6dd]
[runnervm7b5n9:07354] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f208d22a1ca]
[runnervm7b5n9:07354] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f208d22a28b]
[runnervm7b5n9:07354] [11] plumed(+0x15365)[0x563751aff365]
[runnervm7b5n9:07354] *** End of error message ***
</pre>
{% endraw %}
