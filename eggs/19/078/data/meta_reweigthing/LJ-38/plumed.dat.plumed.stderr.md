**Project ID:** [plumID:19.078]({{ '/' | absolute_url }}eggs/19/078/)  
Stderr for source:  meta_reweigthing/LJ-38/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:243) void PLMD::Action::error(const string&) const
ERROR in input to action MATHEVAL with label ns : action nsa has no component named nsa (hint! the components in this actions are: )
[fv-az532-512:10599] *** Process received signal ***
[fv-az532-512:10599] Signal: Aborted (6)
[fv-az532-512:10599] Signal code:  (-6)
[fv-az532-512:10599] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fb3ad642520]
[fv-az532-512:10599] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fb3ad6969fc]
[fv-az532-512:10599] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fb3ad642476]
[fv-az532-512:10599] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fb3ad6287f3]
[fv-az532-512:10599] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7fb3adaa4f26]
[fv-az532-512:10599] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7fb3adab6d9c]
[fv-az532-512:10599] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7fb3adab6e07]
[fv-az532-512:10599] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fb3adab70bb]
[fv-az532-512:10599] [ 8] plumed(+0x12f48)[0x55b54fc2af48]
[fv-az532-512:10599] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fb3ad629d90]
[fv-az532-512:10599] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fb3ad629e40]
[fv-az532-512:10599] [11] plumed(+0x131e5)[0x55b54fc2b1e5]
[fv-az532-512:10599] *** End of error message ***
</pre>
{% endraw %}
