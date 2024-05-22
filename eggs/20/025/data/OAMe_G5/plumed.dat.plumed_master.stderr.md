**Project ID:** [plumID:20.025]({{ '/' | absolute_url }}eggs/20/025/)  
Stderr for source:  OAMe_G5/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::add_buffer_to<std::bad_alloc>'
what():  std::bad_alloc
[fv-az1435-553:42627] *** Process received signal ***
[fv-az1435-553:42627] Signal: Aborted (6)
[fv-az1435-553:42627] Signal code:  (-6)
[fv-az1435-553:42627] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7efd9f442520]
[fv-az1435-553:42627] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7efd9f4969fc]
[fv-az1435-553:42627] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7efd9f442476]
[fv-az1435-553:42627] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7efd9f4287f3]
[fv-az1435-553:42627] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7efd9f8a2b9e]
[fv-az1435-553:42627] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7efd9f8ae20c]
[fv-az1435-553:42627] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7efd9f8ae277]
[fv-az1435-553:42627] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7efd9f8ae52b]
[fv-az1435-553:42627] [ 8] plumed_master(+0x14274)[0x55db04c4a274]
[fv-az1435-553:42627] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7efd9f429d90]
[fv-az1435-553:42627] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7efd9f429e40]
[fv-az1435-553:42627] [11] plumed_master(+0x14ed5)[0x55db04c4aed5]
[fv-az1435-553:42627] *** End of error message ***
</pre>
{% endraw %}
