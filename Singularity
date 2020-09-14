Bootstrap: shub
From: willgpaik/centos7_aci

%environment
        export PATH=$PATH:/opt/sw/visit/bin/

%post
        yum update -y
        yum -y install libfabric-devel

        mkdir -p /opt/sw/
        cd /opt/sw
        wget https://github.com/visit-dav/visit/releases/download/v3.1.2/visit3_1_2.linux-x86_64-rhel7-wmesa.tar.gz
        tar -xf visit3_1_2.linux-x86_64-rhel7-wmesa.tar.gz
        mv visit3_1_2.linux-x86_64 visit
        rm visit3_1_2.linux-x86_64-rhel7-wmesa.tar.gz
