**Project ID:** [plumID:19.078]({{ '/' | absolute_url }}eggs/19/078/)  
Stderr for source:  meta_reweigthing/LJ-38/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at Action.cpp:243, function void PLMD::Action::error(const string&) const
+++ message follows +++
ERROR in input to action MATHEVAL with label ns : action nsa has no component named nsa (hint! the components in this actions are: )
[fv-az99-305:26989] *** Process received signal ***
[fv-az99-305:26989] Signal: Aborted (6)
[fv-az99-305:26989] Signal code:  (-6)
[fv-az99-305:26989] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f8789030210]
[fv-az99-305:26989] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f878903018b]
[fv-az99-305:26989] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f878900f859]
[fv-az99-305:26989] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f8789297951]
[fv-az99-305:26989] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f87892a347c]
[fv-az99-305:26989] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f87892a34e7]
[fv-az99-305:26989] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f87892a3799]
[fv-az99-305:26989] [ 7] plumed(+0xf47d)[0x56434690547d]
[fv-az99-305:26989] [ 8] plumed(+0x14004)[0x56434690a004]
[fv-az99-305:26989] [ 9] plumed(+0xf698)[0x564346905698]
[fv-az99-305:26989] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f87890110b3]
[fv-az99-305:26989] [11] plumed(+0xf76e)[0x56434690576e]
[fv-az99-305:26989] *** End of error message ***
</pre>
{% endraw %}
