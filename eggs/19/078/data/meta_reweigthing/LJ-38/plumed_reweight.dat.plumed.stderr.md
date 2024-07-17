**Project ID:** [plumID:19.078]({{ '/' | absolute_url }}eggs/19/078/)  
Stderr for source:  meta_reweigthing/LJ-38/plumed_reweight.dat   
Download: [zipped raw stdout](plumed_reweight.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_reweight.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action MATHEVAL with label ns : action nsa has no component named nsa (hint! the components in this actions are: )
[fv-az695-456:75831] *** Process received signal ***
[fv-az695-456:75831] Signal: Aborted (6)
[fv-az695-456:75831] Signal code:  (-6)
[fv-az695-456:75831] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f1b2c842520]
[fv-az695-456:75831] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f1b2c8969fc]
[fv-az695-456:75831] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f1b2c842476]
[fv-az695-456:75831] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f1b2c8287f3]
[fv-az695-456:75831] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f1b2cca2b9e]
[fv-az695-456:75831] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f1b2ccae20c]
[fv-az695-456:75831] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f1b2ccae277]
[fv-az695-456:75831] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f1b2ccae52b]
[fv-az695-456:75831] [ 8] plumed(+0x12f48)[0x5575ba161f48]
[fv-az695-456:75831] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f1b2c829d90]
[fv-az695-456:75831] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f1b2c829e40]
[fv-az695-456:75831] [11] plumed(+0x131e5)[0x5575ba1621e5]
[fv-az695-456:75831] *** End of error message ***
</pre>
{% endraw %}
