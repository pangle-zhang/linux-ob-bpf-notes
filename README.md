# linux-ob-bpf-notes

## SLES15 SP4

    zypper in git
    zypper in gcc gcc-c++
    zypper in cmake
    zypper in python

    mkdir llvm-project
    cd llvm-project
    git clone https://github.com/llvm/llvm-project.git .
    mkdir build
    cd build
    cmake -DLLVM_ENABLE_PROJECTS=clang -DCMAKE_BUILD_TYPE=Release -G "Unix Makefiles" ../llvm
    make
    make install

## QA


1. SLES15 SP4 zypper repository

        zypper ar -cfp 90 https://mirrors.aliyun.com/opensuse/distribution/leap/15.4/repo/oss aliyun_repo_oss
        zypper ar -cfp 90 https://mirrors.aliyun.com/opensuse/distribution/leap/15.4/repo/none-oss aliyun_repo_none_oss


3. TBD# linux-ob-bpf-notes
