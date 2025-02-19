**Project ID:** [plumID:21.016]({{ '/' | absolute_url }}eggs/21/016/)  
Stderr for source:  input_files/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action SAXS with label saxs : cannot understand the following words from the input line : SCALEINT=1
[fv-az1770-999:07965] *** Process received signal ***
[fv-az1770-999:07965] Signal: Aborted (6)
[fv-az1770-999:07965] Signal code:  (-6)
[fv-az1770-999:07965] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fbbc8a45330]
[fv-az1770-999:07965] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fbbc8a9eb2c]
[fv-az1770-999:07965] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fbbc8a4527e]
[fv-az1770-999:07965] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fbbc8a288ff]
[fv-az1770-999:07965] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fbbc8ea5ff5]
[fv-az1770-999:07965] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fbbc8ebb0da]
[fv-az1770-999:07965] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fbbc8ea5a55]
[fv-az1770-999:07965] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fbbc8ea5a6f]
[fv-az1770-999:07965] [ 8] plumed_master(+0x146dd)[0x558b37a346dd]
[fv-az1770-999:07965] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fbbc8a2a1ca]
[fv-az1770-999:07965] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fbbc8a2a28b]
[fv-az1770-999:07965] [11] plumed_master(+0x15365)[0x558b37a35365]
[fv-az1770-999:07965] *** End of error message ***
</pre>
{% endraw %}
