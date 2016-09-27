# A Recipe for a haproxy 1.6.9 stable version RPM on CentOS 7

Note: This doesn't build on centos 6 due to required macros and the systemd-units package

Perform the following on a build box as a regular user.

## Create an RPM Build Environment

Install rpmdevtools from the [EPEL][epel] repository:

`$ sudo yum install rpmdevtools pcre-devel`

## Build the RPM

`$ make`

The resulting RPM will be in ~/rpmbuild/RPMS/x86_64

## Credits

Based on the Red Hat 6.4 RPM spec for haproxy 1.4.

Maintained by [Tim Jacomb](t.jacomb@kainos.com)

[EPEL]: http://fedoraproject.org/wiki/EPEL#How_can_I_use_these_extra_packages.3F

Forked from https://github.com/ITV/rpm-haproxy (1.6 but broken now) which was forked from https://github.com/swisstxt/rpm-haproxy (1.6 Dev support) which was Forked from https://github.com/bluerail/haproxy-centos (1.5 Stable support)

