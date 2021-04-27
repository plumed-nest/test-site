**Project ID:** [plumID:19.078]({{ '/' | absolute_url }}eggs/19/078/)  
Stderr for source:  meta_reweigthing/LJ-38/plumed_reweight.dat   
(download [zipped raw stdout](plumed_reweight.dat.plumed.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at Action.cpp:243, function void PLMD::Action::error(const string&) const
+++ message follows +++
ERROR in input to action MATHEVAL with label ns : action nsa has no component named nsa (hint! the components in this actions are: )
[fv-az99-305:27013] *** Process received signal ***
[fv-az99-305:27013] Signal: Aborted (6)
[fv-az99-305:27013] Signal code:  (-6)
[fv-az99-305:27013] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f4a259a2210]
[fv-az99-305:27013] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f4a259a218b]
[fv-az99-305:27013] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f4a25981859]
[fv-az99-305:27013] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f4a25c09951]
[fv-az99-305:27013] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f4a25c1547c]
[fv-az99-305:27013] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f4a25c154e7]
[fv-az99-305:27013] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f4a25c15799]
[fv-az99-305:27013] [ 7] plumed(+0xf47d)[0x55ae55fc647d]
[fv-az99-305:27013] [ 8] plumed(+0x14004)[0x55ae55fcb004]
[fv-az99-305:27013] [ 9] plumed(+0xf698)[0x55ae55fc6698]
[fv-az99-305:27013] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f4a259830b3]
[fv-az99-305:27013] [11] plumed(+0xf76e)[0x55ae55fc676e]
[fv-az99-305:27013] *** End of error message ***
</pre>
{% endraw %}
