**Project ID:** [plumID:21.005]({{ '/' | absolute_url }}eggs/21/005/)  
Stderr for source:  CO2/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:243) void PLMD::Action::error(const string&) const
ERROR in input to action PYTORCH_MODEL with label auto1 : action so has no component named Sk3_-3_-3 (hint! the components in this actions are: so.Sk-[1_-5_-1] so.Sk-[1_-5_1] so.Sk-[1_-1_-5] so.Sk-[1_-1_5] so.Sk-[1_1_-5] so.Sk-[1_1_5] so.Sk-[1_5_-1] so.Sk-[1_5_1] so.Sk-[3_-3_-3] so.Sk-[3_-3_3] so.Sk-[3_3_-3] so.Sk-[3_3_3] so.Sk-[5_-1_-1] so.Sk-[5_-1_1] so.Sk-[5_1_-1] so.Sk-[5_1_1] so.Sk-[0_3_-6] so.Sk-[0_3_6] so.Sk-[0_6_-3] so.Sk-[0_6_3] so.Sk-[2_-5_-4] so.Sk-[2_-5_4] so.Sk-[2_-4_-5] so.Sk-[2_-4_5] so.Sk-[2_4_-5] so.Sk-[2_4_5] so.Sk-[2_5_-4] so.Sk-[2_5_4] so.Sk-[3_-6_0] so.Sk-[3_0_-6] so.Sk-[3_0_6] so.Sk-[3_6_0] so.Sk-[4_-5_-2] so.Sk-[4_-5_2] so.Sk-[4_-2_-5] so.Sk-[4_-2_5] so.Sk-[4_2_-5] so.Sk-[4_2_5] so.Sk-[4_5_-2] so.Sk-[4_5_2] so.Sk-[5_-4_-2] so.Sk-[5_-4_2] so.Sk-[5_-2_-4] so.Sk-[5_-2_4] so.Sk-[5_2_-4] so.Sk-[5_2_4] so.Sk-[5_4_-2] so.Sk-[5_4_2] so.Sk-[6_-3_0] so.Sk-[6_0_-3] so.Sk-[6_0_3] so.Sk-[6_3_0] so.Sk-[1_-7_-2] so.Sk-[1_-7_2] so.Sk-[1_-2_-7] so.Sk-[1_-2_7] so.Sk-[1_2_-7] so.Sk-[1_2_7] so.Sk-[1_7_-2] so.Sk-[1_7_2] so.Sk-[2_-7_-1] so.Sk-[2_-7_1] so.Sk-[2_-5_-5] so.Sk-[2_-5_5] so.Sk-[2_-1_-7] so.Sk-[2_-1_7] so.Sk-[2_1_-7] so.Sk-[2_1_7] so.Sk-[2_5_-5] so.Sk-[2_5_5] so.Sk-[2_7_-1] so.Sk-[2_7_1] so.Sk-[3_-6_-3] so.Sk-[3_-6_3] so.Sk-[3_-3_-6] so.Sk-[3_-3_6] so.Sk-[3_3_-6] so.Sk-[3_3_6] so.Sk-[3_6_-3] so.Sk-[3_6_3] so.Sk-[5_-5_-2] so.Sk-[5_-5_2] so.Sk-[5_-2_-5] so.Sk-[5_-2_5] so.Sk-[5_2_-5] so.Sk-[5_2_5] so.Sk-[5_5_-2] so.Sk-[5_5_2] so.Sk-[6_-3_-3] so.Sk-[6_-3_3] so.Sk-[6_3_-3] so.Sk-[6_3_3] so.Sk-[7_-2_-1] so.Sk-[7_-2_1] so.Sk-[7_-1_-2] so.Sk-[7_-1_2] so.Sk-[7_1_-2] so.Sk-[7_1_2] so.Sk-[7_2_-1] so.Sk-[7_2_1] so.Sk-[0_6_-9] so.Sk-[0_6_9] so.Sk-[0_9_-6] so.Sk-[0_9_6] so.Sk-[1_-10_-4] so.Sk-[1_-10_4] so.Sk-[1_-4_-10] so.Sk-[1_-4_10] so.Sk-[1_4_-10] so.Sk-[1_4_10] so.Sk-[1_10_-4] so.Sk-[1_10_4] so.Sk-[2_-8_-7] so.Sk-[2_-8_7] so.Sk-[2_-7_-8] so.Sk-[2_-7_8] so.Sk-[2_7_-8] so.Sk-[2_7_8] so.Sk-[2_8_-7] so.Sk-[2_8_7] so.Sk-[4_-10_-1] so.Sk-[4_-10_1] so.Sk-[4_-1_-10] so.Sk-[4_-1_10] so.Sk-[4_1_-10] so.Sk-[4_1_10] so.Sk-[4_10_-1] so.Sk-[4_10_1] so.Sk-[6_-9_0] so.Sk-[6_0_-9] so.Sk-[6_0_9] so.Sk-[6_9_0] so.Sk-[7_-8_-2] so.Sk-[7_-8_2] so.Sk-[7_-2_-8] so.Sk-[7_-2_8] so.Sk-[7_2_-8] so.Sk-[7_2_8] so.Sk-[7_8_-2] so.Sk-[7_8_2] so.Sk-[8_-7_-2] so.Sk-[8_-7_2] so.Sk-[8_-2_-7] so.Sk-[8_-2_7] so.Sk-[8_2_-7] so.Sk-[8_2_7] so.Sk-[8_7_-2] so.Sk-[8_7_2] so.Sk-[9_-6_0] so.Sk-[9_0_-6] so.Sk-[9_0_6] so.Sk-[9_6_0] so.Sk-[10_-4_-1] so.Sk-[10_-4_1] so.Sk-[10_-1_-4] so.Sk-[10_-1_4] so.Sk-[10_1_-4] so.Sk-[10_1_4] so.Sk-[10_4_-1] so.Sk-[10_4_1] so.Sk-[1_-11_-2] so.Sk-[1_-11_2] so.Sk-[1_-10_-5] so.Sk-[1_-10_5] so.Sk-[1_-5_-10] so.Sk-[1_-5_10] so.Sk-[1_-2_-11] so.Sk-[1_-2_11] so.Sk-[1_2_-11] so.Sk-[1_2_11] so.Sk-[1_5_-10] so.Sk-[1_5_10] so.Sk-[1_10_-5] so.Sk-[1_10_5] so.Sk-[1_11_-2] so.Sk-[1_11_2] so.Sk-[2_-11_-1] so.Sk-[2_-11_1] so.Sk-[2_-1_-11] so.Sk-[2_-1_11] so.Sk-[2_1_-11] so.Sk-[2_1_11] so.Sk-[2_11_-1] so.Sk-[2_11_1] so.Sk-[3_-9_-6] so.Sk-[3_-9_6] so.Sk-[3_-6_-9] so.Sk-[3_-6_9] so.Sk-[3_6_-9] so.Sk-[3_6_9] so.Sk-[3_9_-6] so.Sk-[3_9_6] so.Sk-[5_-10_-1] so.Sk-[5_-10_1] so.Sk-[5_-1_-10] so.Sk-[5_-1_10] so.Sk-[5_1_-10] so.Sk-[5_1_10] so.Sk-[5_10_-1] so.Sk-[5_10_1] so.Sk-[6_-9_-3] so.Sk-[6_-9_3] so.Sk-[6_-3_-9] so.Sk-[6_-3_9] so.Sk-[6_3_-9] so.Sk-[6_3_9] so.Sk-[6_9_-3] so.Sk-[6_9_3] so.Sk-[9_-6_-3] so.Sk-[9_-6_3] so.Sk-[9_-3_-6] so.Sk-[9_-3_6] so.Sk-[9_3_-6] so.Sk-[9_3_6] so.Sk-[9_6_-3] so.Sk-[9_6_3] so.Sk-[10_-5_-1] so.Sk-[10_-5_1] so.Sk-[10_-1_-5] so.Sk-[10_-1_5] so.Sk-[10_1_-5] so.Sk-[10_1_5] so.Sk-[10_5_-1] so.Sk-[10_5_1] so.Sk-[11_-2_-1] so.Sk-[11_-2_1] so.Sk-[11_-1_-2] so.Sk-[11_-1_2] so.Sk-[11_1_-2] so.Sk-[11_1_2] so.Sk-[11_2_-1] so.Sk-[11_2_1] so.Sk-[0_0_12] so.Sk-[0_12_0] so.Sk-[4_-8_-8] so.Sk-[4_-8_8] so.Sk-[4_8_-8] so.Sk-[4_8_8] so.Sk-[8_-8_-4] so.Sk-[8_-8_4] so.Sk-[8_-4_-8] so.Sk-[8_-4_8] so.Sk-[8_4_-8] so.Sk-[8_4_8] so.Sk-[8_8_-4] so.Sk-[8_8_4] so.Sk-[12_0_0] )
[fv-az695-903:07804] *** Process received signal ***
[fv-az695-903:07804] Signal: Aborted (6)
[fv-az695-903:07804] Signal code:  (-6)
[fv-az695-903:07804] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f724aa42520]
[fv-az695-903:07804] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f724aa969fc]
[fv-az695-903:07804] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f724aa42476]
[fv-az695-903:07804] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f724aa287f3]
[fv-az695-903:07804] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f724aea4f26]
[fv-az695-903:07804] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f724aeb6d9c]
[fv-az695-903:07804] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f724aeb6e07]
[fv-az695-903:07804] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f724aeb70bb]
[fv-az695-903:07804] [ 8] plumed(+0x12f48)[0x56236c74cf48]
[fv-az695-903:07804] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f724aa29d90]
[fv-az695-903:07804] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f724aa29e40]
[fv-az695-903:07804] [11] plumed(+0x131e5)[0x56236c74d1e5]
[fv-az695-903:07804] *** End of error message ***
</pre>
{% endraw %}
