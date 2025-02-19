**Project ID:** [plumID:23.044]({{ '/' | absolute_url }}eggs/23/044/)  
Stderr for source:  plumed_files/reweight_md.dat   
Download: [zipped raw stdout](reweight_md.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](reweight_md.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
WARNING: IFile closed in the middle of reading. seems strange!
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action DUMPGRID with label @32 : keyword ARG is compulsory for this action
[fv-az1326-415:07212] *** Process received signal ***
[fv-az1326-415:07212] Signal: Aborted (6)
[fv-az1326-415:07212] Signal code:  (-6)
[fv-az1326-415:07212] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f977aa45330]
[fv-az1326-415:07212] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f977aa9eb2c]
[fv-az1326-415:07212] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f977aa4527e]
[fv-az1326-415:07212] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f977aa288ff]
[fv-az1326-415:07212] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f977aea5ff5]
[fv-az1326-415:07212] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f977aebb0da]
[fv-az1326-415:07212] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f977aea5a55]
[fv-az1326-415:07212] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f977aea5a6f]
[fv-az1326-415:07212] [ 8] plumed_master(+0x146dd)[0x55f651bf46dd]
[fv-az1326-415:07212] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f977aa2a1ca]
[fv-az1326-415:07212] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f977aa2a28b]
[fv-az1326-415:07212] [11] plumed_master(+0x15365)[0x55f651bf5365]
[fv-az1326-415:07212] *** End of error message ***
</pre>
{% endraw %}
