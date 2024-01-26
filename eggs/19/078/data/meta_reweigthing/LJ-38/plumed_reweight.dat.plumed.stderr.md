**Project ID:** [plumID:19.078]({{ '/' | absolute_url }}eggs/19/078/)  
Stderr for source:  meta_reweigthing/LJ-38/plumed_reweight.dat   
Download: [zipped raw stdout](plumed_reweight.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_reweight.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:243) void PLMD::Action::error(const string&) const
ERROR in input to action MATHEVAL with label ns : action nsa has no component named nsa (hint! the components in this actions are: )
[fv-az532-512:10631] *** Process received signal ***
[fv-az532-512:10631] Signal: Aborted (6)
[fv-az532-512:10631] Signal code:  (-6)
[fv-az532-512:10631] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7ffa30e42520]
[fv-az532-512:10631] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7ffa30e969fc]
[fv-az532-512:10631] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7ffa30e42476]
[fv-az532-512:10631] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7ffa30e287f3]
[fv-az532-512:10631] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7ffa312a4f26]
[fv-az532-512:10631] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7ffa312b6d9c]
[fv-az532-512:10631] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7ffa312b6e07]
[fv-az532-512:10631] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7ffa312b70bb]
[fv-az532-512:10631] [ 8] plumed(+0x12f48)[0x55ba29efff48]
[fv-az532-512:10631] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7ffa30e29d90]
[fv-az532-512:10631] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7ffa30e29e40]
[fv-az532-512:10631] [11] plumed(+0x131e5)[0x55ba29f001e5]
[fv-az532-512:10631] *** End of error message ***
</pre>
{% endraw %}
