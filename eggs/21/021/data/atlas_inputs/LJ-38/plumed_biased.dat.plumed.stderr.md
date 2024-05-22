**Project ID:** [plumID:21.021]({{ '/' | absolute_url }}eggs/21/021/)  
Stderr for source:  atlas_inputs/LJ-38/plumed_biased.dat   
Download: [zipped raw stdout](plumed_biased.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_biased.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action MATHEVAL with label n4 : action nsa has no component named nsa (hint! the components in this actions are: )
[fv-az1543-369:41304] *** Process received signal ***
[fv-az1543-369:41304] Signal: Aborted (6)
[fv-az1543-369:41304] Signal code:  (-6)
[fv-az1543-369:41304] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f43e1a42520]
[fv-az1543-369:41304] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f43e1a969fc]
[fv-az1543-369:41304] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f43e1a42476]
[fv-az1543-369:41304] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f43e1a287f3]
[fv-az1543-369:41304] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f43e1ea2b9e]
[fv-az1543-369:41304] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f43e1eae20c]
[fv-az1543-369:41304] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f43e1eae277]
[fv-az1543-369:41304] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f43e1eae52b]
[fv-az1543-369:41304] [ 8] plumed(+0x12f48)[0x56048b554f48]
[fv-az1543-369:41304] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f43e1a29d90]
[fv-az1543-369:41304] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f43e1a29e40]
[fv-az1543-369:41304] [11] plumed(+0x131e5)[0x56048b5551e5]
[fv-az1543-369:41304] *** End of error message ***
</pre>
{% endraw %}
