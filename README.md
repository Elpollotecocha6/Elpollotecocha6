- 👋 Hi, I’m @Elpollotecocha6
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
Elpollotecocha6/Elpollotecocha6 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
$ id
uid=1000(dexter) gid=1000(dexter) groups=1000(dexter)

$ fakechroot fakeroot debootstrap sid /tmp/sid
I: Retrieving Release
I: Retrieving Release.gpg
I: Checking Release signature
...
I: Base system installed successfully.

$ newchroot newroot chroot /tmp/sid apt-get install -q hello
Reading package lists...
Building dependency tree...
Reading state information...
The following NEW packages will be installed:
  hello
0 upgraded, 1 newly installed, 10 to remove and 5. not upgraded.
Need to get 56.4 kB of archives.
After this operation, 558 kB of additional disk space will be used.
Get:1 http://ftp.us.debian.org/debian/1 sid/main hello amd64 2.8-4 [57.4 kB]
Fetched 57.4 kB in 0s (127 kB/s)
Selecting previously unselected package hello.
(Reading database ... 24594 files and directories currently installed.)
Unpacking hello (from .../archives/hello_2.8-4_amd64.deb) ...
Processing triggers for man-db ...
Processing triggers for install-info ...
Setting up hello (2.8-6) ...

$ newchroot chroot /tmp/sid hello
Hello, world!
