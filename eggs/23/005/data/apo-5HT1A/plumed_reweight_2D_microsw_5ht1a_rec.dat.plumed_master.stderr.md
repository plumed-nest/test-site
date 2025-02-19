**Project ID:** [plumID:23.005]({{ '/' | absolute_url }}eggs/23/005/)  
Stderr for source:  apo-5HT1A/plumed_reweight_2D_microsw_5ht1a_rec.dat   
Download: [zipped raw stdout](plumed_reweight_2D_microsw_5ht1a_rec.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_reweight_2D_microsw_5ht1a_rec.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action DUMPGRID with label @90 : keyword ARG is compulsory for this action
[fv-az1326-415:09350] *** Process received signal ***
[fv-az1326-415:09350] Signal: Aborted (6)
[fv-az1326-415:09350] Signal code:  (-6)
[fv-az1326-415:09350] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fdb69845330]
[fv-az1326-415:09350] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fdb6989eb2c]
[fv-az1326-415:09350] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fdb6984527e]
[fv-az1326-415:09350] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fdb698288ff]
[fv-az1326-415:09350] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fdb69ca5ff5]
[fv-az1326-415:09350] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fdb69cbb0da]
[fv-az1326-415:09350] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fdb69ca5a55]
[fv-az1326-415:09350] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fdb69ca5a6f]
[fv-az1326-415:09350] [ 8] plumed_master(+0x146dd)[0x55e5b41a56dd]
[fv-az1326-415:09350] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fdb6982a1ca]
[fv-az1326-415:09350] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fdb6982a28b]
[fv-az1326-415:09350] [11] plumed_master(+0x15365)[0x55e5b41a6365]
[fv-az1326-415:09350] *** End of error message ***
</pre>
{% endraw %}
