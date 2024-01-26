**Project ID:** [plumID:19.078]({{ '/' | absolute_url }}eggs/19/078/)  
Stderr for source:  meta_reweigthing/LJ-38/plumed_reweight.dat   
Download: [zipped raw stdout](plumed_reweight.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_reweight.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:288) void PLMD::Action::error(const string&) const
ERROR in input to action MATHEVAL with label ns : action nsa has no component named nsa (hint! the components in this actions are: )
[fv-az532-512:10639] *** Process received signal ***
[fv-az532-512:10639] Signal: Aborted (6)
[fv-az532-512:10639] Signal code:  (-6)
[fv-az532-512:10639] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7ffb46842520]
[fv-az532-512:10639] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7ffb468969fc]
[fv-az532-512:10639] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7ffb46842476]
[fv-az532-512:10639] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7ffb468287f3]
[fv-az532-512:10639] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7ffb46ca4f26]
[fv-az532-512:10639] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7ffb46cb6d9c]
[fv-az532-512:10639] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7ffb46cb6e07]
[fv-az532-512:10639] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7ffb46cb70bb]
[fv-az532-512:10639] [ 8] plumed_master(+0x12ebf)[0x5556e9cbfebf]
[fv-az532-512:10639] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7ffb46829d90]
[fv-az532-512:10639] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7ffb46829e40]
[fv-az532-512:10639] [11] plumed_master(+0x13155)[0x5556e9cc0155]
[fv-az532-512:10639] *** End of error message ***
</pre>
{% endraw %}
