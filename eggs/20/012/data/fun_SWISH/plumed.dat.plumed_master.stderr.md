**Project ID:** [plumID:20.012]({{ '/' | absolute_url }}eggs/20/012/)  
Stderr for source:  fun_SWISH/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at IFile.cpp:113, function virtual PLMD::IFile& PLMD::IFile::open(const string&)
+++ assertion failed: do_exist
+++ message follows +++
file cmap.dat cannot be found
[fv-az99-305:23499] *** Process received signal ***
[fv-az99-305:23499] Signal: Aborted (6)
[fv-az99-305:23499] Signal code:  (-6)
[fv-az99-305:23499] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f3f7849d210]
[fv-az99-305:23499] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f3f7849d18b]
[fv-az99-305:23499] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f3f7847c859]
[fv-az99-305:23499] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f3f78704951]
[fv-az99-305:23499] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f3f7871047c]
[fv-az99-305:23499] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f3f787104e7]
[fv-az99-305:23499] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7f3f787107ed]
[fv-az99-305:23499] [ 7] plumed_master(+0xf568)[0x5557423cd568]
[fv-az99-305:23499] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f3f7847e0b3]
[fv-az99-305:23499] [ 9] plumed_master(+0xf79e)[0x5557423cd79e]
[fv-az99-305:23499] *** End of error message ***
</pre>
{% endraw %}
