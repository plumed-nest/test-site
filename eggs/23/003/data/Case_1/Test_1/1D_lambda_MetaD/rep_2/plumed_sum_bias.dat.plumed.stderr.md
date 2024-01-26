**Project ID:** [plumID:23.003]({{ '/' | absolute_url }}eggs/23/003/)  
Stderr for source:  Case_1/Test_1/1D_lambda_MetaD/rep_2/plumed_sum_bias.dat   
Download: [zipped raw stdout](plumed_sum_bias.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_sum_bias.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
WARNING: IFile closed in the middle of reading. seems strange!
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:243) void PLMD::Action::error(const string&) const
ERROR in input to action METAD with label metad : restart file HILLS_LAMBDA_modified_fake not found
[fv-az979-741:04807] *** Process received signal ***
[fv-az979-741:04807] Signal: Aborted (6)
[fv-az979-741:04807] Signal code:  (-6)
[fv-az979-741:04807] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f68bde42520]
[fv-az979-741:04807] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f68bde969fc]
[fv-az979-741:04807] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f68bde42476]
[fv-az979-741:04807] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f68bde287f3]
[fv-az979-741:04807] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f68be2a4f26]
[fv-az979-741:04807] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f68be2b6d9c]
[fv-az979-741:04807] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f68be2b6e07]
[fv-az979-741:04807] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f68be2b70bb]
[fv-az979-741:04807] [ 8] plumed(+0x12f48)[0x5647d34e7f48]
[fv-az979-741:04807] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f68bde29d90]
[fv-az979-741:04807] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f68bde29e40]
[fv-az979-741:04807] [11] plumed(+0x131e5)[0x5647d34e81e5]
[fv-az979-741:04807] *** End of error message ***
</pre>
{% endraw %}
