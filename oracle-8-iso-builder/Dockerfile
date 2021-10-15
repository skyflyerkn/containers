FROM oraclelinux:8
MAINTAINER skyflyerkn@gmail.com
RUN curl -L -o /root/OL8-U4-x86_64-boot.iso https://yum.oracle.com/ISOS/OracleLinux/OL8/u4/x86_64/x86_64-boot.iso
RUN echo $(sha256sum /root/OL8-U4-x86_64-boot.iso)
RUN dnf update -y
RUN dnf install -y yum-utils createrepo syslinux genisoimage isomd5sum bzip2 curl file git wget unzip rsync
CMD ["/bin/bash"]