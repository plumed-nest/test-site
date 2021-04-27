**Project ID:** [plumID:20.027]({{ '/' | absolute_url }}eggs/20/027/)  
Stderr for source:  MetaD_script.dat   
(download [zipped raw stdout](MetaD_script.dat.plumed_master.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at Action.cpp:243, function void PLMD::Action::error(const string&) const
+++ message follows +++
ERROR in input to action METAD with label metad : When using ADAPTIVE Gaussians on a grid SIGMA_MIN must be specified
[fv-az99-305:21513] *** Process received signal ***
[fv-az99-305:21513] Signal: Aborted (6)
[fv-az99-305:21513] Signal code:  (-6)
[fv-az99-305:21513] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f425d551210]
[fv-az99-305:21513] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f425d55118b]
[fv-az99-305:21513] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f425d530859]
[fv-az99-305:21513] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f425d7b8951]
[fv-az99-305:21513] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f425d7c447c]
[fv-az99-305:21513] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f425d7c44e7]
[fv-az99-305:21513] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7f425d7c47ed]
[fv-az99-305:21513] [ 7] plumed_master(+0xf568)[0x55c084239568]
[fv-az99-305:21513] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f425d5320b3]
[fv-az99-305:21513] [ 9] plumed_master(+0xf79e)[0x55c08423979e]
[fv-az99-305:21513] *** End of error message ***
</pre>
{% endraw %}
