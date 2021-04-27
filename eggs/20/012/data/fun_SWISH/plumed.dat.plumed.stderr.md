**Project ID:** [plumID:20.012]({{ '/' | absolute_url }}eggs/20/012/)  
Stderr for source:  fun_SWISH/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at IFile.cpp:113, function virtual PLMD::IFile& PLMD::IFile::open(const string&)
+++ assertion failed: do_exist
+++ message follows +++
file cmap.dat cannot be found
[fv-az99-305:23480] *** Process received signal ***
[fv-az99-305:23480] Signal: Aborted (6)
[fv-az99-305:23480] Signal code:  (-6)
[fv-az99-305:23480] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f6bd39e7210]
[fv-az99-305:23480] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f6bd39e718b]
[fv-az99-305:23480] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f6bd39c6859]
[fv-az99-305:23480] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f6bd3c4e951]
[fv-az99-305:23480] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f6bd3c5a47c]
[fv-az99-305:23480] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f6bd3c5a4e7]
[fv-az99-305:23480] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f6bd3c5a799]
[fv-az99-305:23480] [ 7] plumed(+0xf47d)[0x55b482bd547d]
[fv-az99-305:23480] [ 8] plumed(+0x14004)[0x55b482bda004]
[fv-az99-305:23480] [ 9] plumed(+0xf698)[0x55b482bd5698]
[fv-az99-305:23480] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f6bd39c80b3]
[fv-az99-305:23480] [11] plumed(+0xf76e)[0x55b482bd576e]
[fv-az99-305:23480] *** End of error message ***
</pre>
{% endraw %}
