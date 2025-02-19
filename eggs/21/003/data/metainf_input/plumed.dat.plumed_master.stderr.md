**Project ID:** [plumID:21.003]({{ '/' | absolute_url }}eggs/21/003/)  
Stderr for source:  metainf_input/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action SAXS with label test2 : cannot understand the following words from the input line : SCALEINT=1680
[fv-az1436-30:10592] *** Process received signal ***
[fv-az1436-30:10592] Signal: Aborted (6)
[fv-az1436-30:10592] Signal code:  (-6)
[fv-az1436-30:10592] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fc3cc645330]
[fv-az1436-30:10592] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fc3cc69eb2c]
[fv-az1436-30:10592] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fc3cc64527e]
[fv-az1436-30:10592] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fc3cc6288ff]
[fv-az1436-30:10592] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fc3ccaa5ff5]
[fv-az1436-30:10592] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fc3ccabb0da]
[fv-az1436-30:10592] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fc3ccaa5a55]
[fv-az1436-30:10592] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fc3ccaa5a6f]
[fv-az1436-30:10592] [ 8] plumed_master(+0x146dd)[0x556b493676dd]
[fv-az1436-30:10592] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fc3cc62a1ca]
[fv-az1436-30:10592] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fc3cc62a28b]
[fv-az1436-30:10592] [11] plumed_master(+0x15365)[0x556b49368365]
[fv-az1436-30:10592] *** End of error message ***
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action SAXS with label test2 : cannot understand the following words from the input line : SCALEINT=1680
[fv-az1436-30:10591] *** Process received signal ***
[fv-az1436-30:10591] Signal: Aborted (6)
[fv-az1436-30:10591] Signal code:  (-6)
[fv-az1436-30:10591] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fd481e45330]
[fv-az1436-30:10591] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fd481e9eb2c]
[fv-az1436-30:10591] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fd481e4527e]
[fv-az1436-30:10591] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fd481e288ff]
[fv-az1436-30:10591] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fd4822a5ff5]
[fv-az1436-30:10591] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fd4822bb0da]
[fv-az1436-30:10591] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fd4822a5a55]
[fv-az1436-30:10591] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fd4822a5a6f]
[fv-az1436-30:10591] [ 8] plumed_master(+0x146dd)[0x5583f03256dd]
[fv-az1436-30:10591] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fd481e2a1ca]
[fv-az1436-30:10591] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fd481e2a28b]
[fv-az1436-30:10591] [11] plumed_master(+0x15365)[0x5583f0326365]
[fv-az1436-30:10591] *** End of error message ***
--------------------------------------------------------------------------
Primary job  terminated normally, but 1 process returned
a non-zero exit code. Per user-direction, the job has been aborted.
--------------------------------------------------------------------------
--------------------------------------------------------------------------
mpirun noticed that process rank 1 with PID 0 on node fv-az1436-30 exited on signal 6 (Aborted).
--------------------------------------------------------------------------
</pre>
{% endraw %}
