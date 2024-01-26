**Project ID:** [plumID:20.029]({{ '/' | absolute_url }}eggs/20/029/)  
Stderr for source:  E2F1-DP1_PLUMED-NEST/MULTI_REPLICA/plumed-main.dat   
Download: [zipped raw stdout](plumed-main.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed-main.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:243) void PLMD::Action::error(const string&) const
ERROR in input to action SAXS with label saxsCG : cannot understand the following words from the input line : SCALEINT=107.069000
[fv-az1542-52:07887] *** Process received signal ***
[fv-az1542-52:07887] Signal: Aborted (6)
[fv-az1542-52:07887] Signal code:  (-6)
[fv-az1542-52:07887] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f589a842520]
[fv-az1542-52:07887] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f589a8969fc]
[fv-az1542-52:07887] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f589a842476]
[fv-az1542-52:07887] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f589a8287f3]
[fv-az1542-52:07887] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f589aca4f26]
[fv-az1542-52:07887] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f589acb6d9c]
[fv-az1542-52:07887] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f589acb6e07]
[fv-az1542-52:07887] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f589acb70bb]
[fv-az1542-52:07887] [ 8] plumed(+0x12f48)[0x55ee81060f48]
[fv-az1542-52:07887] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f589a829d90]
[fv-az1542-52:07887] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f589a829e40]
[fv-az1542-52:07887] [11] plumed(+0x131e5)[0x55ee810611e5]
[fv-az1542-52:07887] *** End of error message ***
</pre>
{% endraw %}
