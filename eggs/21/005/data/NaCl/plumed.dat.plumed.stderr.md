**Project ID:** [plumID:21.005]({{ '/' | absolute_url }}eggs/21/005/)  
Stderr for source:  NaCl/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action PYTORCH_MODEL with label auto1 : action s1 has no component named Sk3_-3_-3 (hint! the components in this actions are: s1.Sk-[1_-5_-1] s1.Sk-[1_-5_1] s1.Sk-[1_-1_-5] s1.Sk-[1_-1_5] s1.Sk-[1_1_-5] s1.Sk-[1_1_5] s1.Sk-[1_5_-1] s1.Sk-[1_5_1] s1.Sk-[3_-3_-3] s1.Sk-[3_-3_3] s1.Sk-[3_3_-3] s1.Sk-[3_3_3] s1.Sk-[5_-1_-1] s1.Sk-[5_-1_1] s1.Sk-[5_1_-1] s1.Sk-[5_1_1] s1.Sk-[0_0_6] s1.Sk-[0_6_0] s1.Sk-[2_-4_-4] s1.Sk-[2_-4_4] s1.Sk-[2_4_-4] s1.Sk-[2_4_4] s1.Sk-[4_-4_-2] s1.Sk-[4_-4_2] s1.Sk-[4_-2_-4] s1.Sk-[4_-2_4] s1.Sk-[4_2_-4] s1.Sk-[4_2_4] s1.Sk-[4_4_-2] s1.Sk-[4_4_2] s1.Sk-[6_0_0] s1.Sk-[0_6_-6] s1.Sk-[0_6_6] s1.Sk-[2_-8_-2] s1.Sk-[2_-8_2] s1.Sk-[2_-2_-8] s1.Sk-[2_-2_8] s1.Sk-[2_2_-8] s1.Sk-[2_2_8] s1.Sk-[2_8_-2] s1.Sk-[2_8_2] s1.Sk-[6_-6_0] s1.Sk-[6_0_-6] s1.Sk-[6_0_6] s1.Sk-[6_6_0] s1.Sk-[8_-2_-2] s1.Sk-[8_-2_2] s1.Sk-[8_2_-2] s1.Sk-[8_2_2] s1.Sk-[1_-7_-7] s1.Sk-[1_-7_7] s1.Sk-[1_7_-7] s1.Sk-[1_7_7] s1.Sk-[3_-9_-3] s1.Sk-[3_-9_3] s1.Sk-[3_-3_-9] s1.Sk-[3_-3_9] s1.Sk-[3_3_-9] s1.Sk-[3_3_9] s1.Sk-[3_9_-3] s1.Sk-[3_9_3] s1.Sk-[5_-7_-5] s1.Sk-[5_-7_5] s1.Sk-[5_-5_-7] s1.Sk-[5_-5_7] s1.Sk-[5_5_-7] s1.Sk-[5_5_7] s1.Sk-[5_7_-5] s1.Sk-[5_7_5] s1.Sk-[7_-7_-1] s1.Sk-[7_-7_1] s1.Sk-[7_-5_-5] s1.Sk-[7_-5_5] s1.Sk-[7_-1_-7] s1.Sk-[7_-1_7] s1.Sk-[7_1_-7] s1.Sk-[7_1_7] s1.Sk-[7_5_-5] s1.Sk-[7_5_5] s1.Sk-[7_7_-1] s1.Sk-[7_7_1] s1.Sk-[9_-3_-3] s1.Sk-[9_-3_3] s1.Sk-[9_3_-3] s1.Sk-[9_3_3] )
[fv-az659-568:43105] *** Process received signal ***
[fv-az659-568:43105] Signal: Aborted (6)
[fv-az659-568:43105] Signal code:  (-6)
[fv-az659-568:43105] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f17a9842520]
[fv-az659-568:43105] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f17a98969fc]
[fv-az659-568:43105] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f17a9842476]
[fv-az659-568:43105] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f17a98287f3]
[fv-az659-568:43105] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f17a9ca2b9e]
[fv-az659-568:43105] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f17a9cae20c]
[fv-az659-568:43105] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f17a9cae277]
[fv-az659-568:43105] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f17a9cae52b]
[fv-az659-568:43105] [ 8] plumed(+0x12f48)[0x560136967f48]
[fv-az659-568:43105] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f17a9829d90]
[fv-az659-568:43105] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f17a9829e40]
[fv-az659-568:43105] [11] plumed(+0x131e5)[0x5601369681e5]
[fv-az659-568:43105] *** End of error message ***
</pre>
{% endraw %}
