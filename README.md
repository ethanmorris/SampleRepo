Sample Repo / Hello World Program
=================================

Your repository should contain your feed with subdirectories: 'files' (containing config), and 'prebuilt' (containing IPKs for the corresponding architecture). The example program is as follows:

/feed/Makefile
/feed/files/config
/feed/prebuilt/ipq806x/hworld.0.0.1_ipq806x.ipk
/feed/prebuilt/ar71xx/hworld.0.0.1_ar71xx.ipk

=================================

To build the example program:

From build root, add this line to feeds.conf:

src-git SampleRepo https://github.com/ethanmorris/SampleRepo

make package/symlinks
make menuconfig
Sample > Apps > hworld
