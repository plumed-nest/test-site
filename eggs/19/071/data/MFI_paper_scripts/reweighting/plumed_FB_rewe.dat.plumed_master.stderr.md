**Project ID:** [plumID:19.071]({{ '/' | absolute_url }}eggs/19/071/)  
Stderr for source:  MFI_paper_scripts/reweighting/plumed_FB_rewe.dat   
(download [zipped raw stdout](plumed_FB_rewe.dat.plumed_master.stdout.txt.zip))  
{% raw %}
<pre>
WARNING: IFile closed in the middle of reading. seems strange!
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at Grid.cpp:565, function static std::unique_ptr<PLMD::GridBase> PLMD::GridBase::create(const string&, const std::vector<PLMD::Value*>&, PLMD::IFile&, bool, bool, bool)
+++ assertion failed: ifile.FieldExist( funcl )
+++ message follows +++
no column labelled metad.bias in in grid input
[fv-az99-305:31655] *** Process received signal ***
[fv-az99-305:31655] Signal: Aborted (6)
[fv-az99-305:31655] Signal code:  (-6)
[fv-az99-305:31655] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f5e6887a210]
[fv-az99-305:31655] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f5e6887a18b]
[fv-az99-305:31655] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f5e68859859]
[fv-az99-305:31655] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f5e68ae1951]
[fv-az99-305:31655] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f5e68aed47c]
[fv-az99-305:31655] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f5e68aed4e7]
[fv-az99-305:31655] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7f5e68aed7ed]
[fv-az99-305:31655] [ 7] plumed_master(+0xf568)[0x5614d514f568]
[fv-az99-305:31655] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f5e6885b0b3]
[fv-az99-305:31655] [ 9] plumed_master(+0xf79e)[0x5614d514f79e]
[fv-az99-305:31655] *** End of error message ***
</pre>
{% endraw %}
