# Perl
**The Perl Language by Larry Wall**

This is an unofficial verbatim redistribution of the binary&source form of the Perl under its open source license (GPL 1.0) terms (see the LICENSE file).

This redistribution is under the same license as the original.

Please visit the official website for more details: https://www.perl.org

## Download
You can download the compiled binary files at the [release page](https://github.com/yuhangwang/Perl/releases).

## Compilation notes
### Compilation environment
* CentOS 6.6
* x86_64 architecture
* Compiler: gcc version 4.4.7 20120313 (Red Hat 4.4.7-11)

### Compilation steps
#### Version: 5.22.0 (2015)
```bash
wget http://www.cpan.org/src/5.0/perl-5.22.0.tar.gz
tar xvf perl-5.22.0
cd perl-5.22.0
./Configure -des --Dprefix=/home/steven/install/perl/5.22.0
make -j16
make test -j16 | tee QualityVerification.txt
make install
```

### Quality verification
Results:
- **All tests successful**
- **Time cost: 867 sec**
- **u=8.56  s=2.76  cu=408.09  cs=47.06  scripts=2223  tests=708759**

See the "QualityVerification.txt" for the output of "make check".
