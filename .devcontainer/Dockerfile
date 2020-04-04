#-------------------------------------------------------------------------------------------------------------
# Copyright (c) Microsoft Corporation. All rights reserved.
# Licensed under the MIT License. See https://go.microsoft.com/fwlink/?linkid=2090316 for license information.
#-------------------------------------------------------------------------------------------------------------

FROM openfoamplus/of_v1906_centos73

ARG username=ofuser
ENV USER=$username 

RUN    yum install -y gdb \
    && echo "$username ALL=(ALL) NOPASSWD:ALL" >> /etc/sudoers

USER $username
