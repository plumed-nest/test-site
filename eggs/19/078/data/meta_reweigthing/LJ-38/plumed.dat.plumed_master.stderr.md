**Project ID:** [plumID:19.078]({{ '/' | absolute_url }}eggs/19/078/)  
Stderr for source:  meta_reweigthing/LJ-38/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at Action.cpp:243, function void PLMD::Action::error(const string&) const
+++ message follows +++
ERROR in input to action MATHEVAL with label ns : action nsa has no component named nsa (hint! the components in this actions are: )
[fv-az99-305:26997] *** Process received signal ***
[fv-az99-305:26997] Signal: Aborted (6)
[fv-az99-305:26997] Signal code:  (-6)
[fv-az99-305:26997] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f2845041210]
[fv-az99-305:26997] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f284504118b]
[fv-az99-305:26997] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f2845020859]
[fv-az99-305:26997] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f28452a8951]
[fv-az99-305:26997] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f28452b447c]
[fv-az99-305:26997] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f28452b44e7]
[fv-az99-305:26997] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7f28452b47ed]
[fv-az99-305:26997] [ 7] plumed_master(+0xf568)[0x560b85a80568]
[fv-az99-305:26997] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f28450220b3]
[fv-az99-305:26997] [ 9] plumed_master(+0xf79e)[0x560b85a8079e]
[fv-az99-305:26997] *** End of error message ***
</pre>
{% endraw %}
