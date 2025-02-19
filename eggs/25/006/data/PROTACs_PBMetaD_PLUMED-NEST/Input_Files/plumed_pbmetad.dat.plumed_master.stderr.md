**Project ID:** [plumID:25.006]({{ '/' | absolute_url }}eggs/25/006/)  
Stderr for source:  PROTACs_PBMetaD_PLUMED-NEST/Input_Files/plumed_pbmetad.dat   
Download: [zipped raw stdout](plumed_pbmetad.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_pbmetad.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action PRINT with label @115 : cannot find action named energy (hint! the actions with value in this ActionSet are: timestep kBT posx posy posz Masses Charges Box driver tbut s_vhl n_vhl ph_brd4 ph_vhl S_5ring_brd4 N_ring_brd4 N_5ring_brd4 linker d_tbut_ph_brd4 d_tbut_S_5ring_brd4 d_tbut_N_ring_brd4 d_tbut_N_5ring_brd4 d_ph_brd4_linker d_ph_vhl_linker d_ph_brd4_ph_vhl d_ph_vhl_S_5ring_brd4 d_ph_vhl_N_ring_brd4 d_ph_vhl_N_5ring_brd4 d_s_vhl_ph_brd4 d_s_S_5ring_brd4 d_s_N_ring_brd4 d_s_N_5ring_brd4 d_n_vhl_ph_brd4 d_n_vhl_S_5ring_brd4 d_n_vhl_N_ring_brd4 d_n_vhl_N_5ring_brd4 rgyr t_brd4_1 t_brd4_2 t_brd4_3 t_brd4_4 t_brd4_5 t_brd4_6 t_brd4_7 t_linker_1 t_linker_2 t_linker_3 t_linker_4 t_linker_5 t_linker_6 t_linker_7 t_linker_8 t_linker_9 t_vhl_1 t_vhl_2 t_vhl_3 t_vhl_4 t_vhl_5 t_vhl_6 t_vhl_7 t_vhl_8 t_vhl_9 t_vhl_10 t_vhl_11 t_vhl_12 t_vhl_13 pbmetad )
[fv-az1770-999:05345] *** Process received signal ***
[fv-az1770-999:05345] Signal: Aborted (6)
[fv-az1770-999:05345] Signal code:  (-6)
[fv-az1770-999:05345] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f0531a45330]
[fv-az1770-999:05345] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f0531a9eb2c]
[fv-az1770-999:05345] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f0531a4527e]
[fv-az1770-999:05345] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f0531a288ff]
[fv-az1770-999:05345] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f0531ea5ff5]
[fv-az1770-999:05345] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f0531ebb0da]
[fv-az1770-999:05345] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f0531ea5a55]
[fv-az1770-999:05345] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f0531ea5a6f]
[fv-az1770-999:05345] [ 8] plumed_master(+0x146dd)[0x55bab116e6dd]
[fv-az1770-999:05345] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f0531a2a1ca]
[fv-az1770-999:05345] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f0531a2a28b]
[fv-az1770-999:05345] [11] plumed_master(+0x15365)[0x55bab116f365]
[fv-az1770-999:05345] *** End of error message ***
</pre>
{% endraw %}
