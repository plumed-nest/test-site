**Project ID:** [plumID:19.071]({{ '/' | absolute_url }}eggs/19/071/)  
Stderr for source:  MFI_paper_scripts/reweighting/plumed_REWE.dat   
(download [zipped raw stdout](plumed_REWE.dat.plumed.stdout.txt.zip))  
{% raw %}
<pre>
WARNING: IFile closed in the middle of reading. seems strange!
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at Action.cpp:243, function void PLMD::Action::error(const string&) const
+++ message follows +++
ERROR in input to action METAD with label metad : cannot understand the following words from the input line : REWEIGHTING_NGRID=200, REWEIGHTING_NHILLS=10
[fv-az99-305:31672] *** Process received signal ***
[fv-az99-305:31672] Signal: Aborted (6)
[fv-az99-305:31672] Signal code:  (-6)
[fv-az99-305:31672] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f9782b03210]
[fv-az99-305:31672] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f9782b0318b]
[fv-az99-305:31672] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f9782ae2859]
[fv-az99-305:31672] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f9782d6a951]
[fv-az99-305:31672] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f9782d7647c]
[fv-az99-305:31672] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f9782d764e7]
[fv-az99-305:31672] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f9782d76799]
[fv-az99-305:31672] [ 7] plumed(+0xf47d)[0x561c1f12447d]
[fv-az99-305:31672] [ 8] plumed(+0x14004)[0x561c1f129004]
[fv-az99-305:31672] [ 9] plumed(+0xf698)[0x561c1f124698]
[fv-az99-305:31672] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f9782ae40b3]
[fv-az99-305:31672] [11] plumed(+0xf76e)[0x561c1f12476e]
[fv-az99-305:31672] *** End of error message ***
</pre>
{% endraw %}
