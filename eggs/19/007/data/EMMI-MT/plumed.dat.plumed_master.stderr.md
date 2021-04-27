**Project ID:** [plumID:19.007]({{ '/' | absolute_url }}eggs/19/007/)  
Stderr for source:  EMMI-MT/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at Action.cpp:243, function void PLMD::Action::error(const string&) const
+++ message follows +++
ERROR in input to action WHOLEMOLECULES with label @4 : cannot understand the following words from the input line : REF0=3.217,4.340,6.195
[fv-az99-305:43862] *** Process received signal ***
[fv-az99-305:43862] Signal: Aborted (6)
[fv-az99-305:43862] Signal code:  (-6)
[fv-az99-305:43862] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fc1fbb49210]
[fv-az99-305:43862] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fc1fbb4918b]
[fv-az99-305:43862] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fc1fbb28859]
[fv-az99-305:43862] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fc1fbdb0951]
[fv-az99-305:43862] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fc1fbdbc47c]
[fv-az99-305:43862] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fc1fbdbc4e7]
[fv-az99-305:43862] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7fc1fbdbc7ed]
[fv-az99-305:43862] [ 7] plumed_master(+0xf568)[0x55a9c6b2f568]
[fv-az99-305:43862] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fc1fbb2a0b3]
[fv-az99-305:43862] [ 9] plumed_master(+0xf79e)[0x55a9c6b2f79e]
[fv-az99-305:43862] *** End of error message ***
</pre>
{% endraw %}
