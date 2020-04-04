#-------------------------------------------------------------------------------------------------------------
# Copyright (c) Microsoft Corporation. All rights reserved.
# Licensed under the MIT License. See https://go.microsoft.com/fwlink/?linkid=2090316 for license information.
#-------------------------------------------------------------------------------------------------------------

FROM openfoamplus/of_v1906_centos73

RUN yum install -y gdb

RUN echo "ofuser ALL=(ALL) NOPASSWD:ALL" >> /etc/sudoers

USER ofuser
