# Supported Log Formats
lnav supports several log formats, that it automatically detects while parsing your logs.<br>
That means if your log file originated from one of those sources, you can already work with them without needing to set up anything extra.

| Name                                  | Table Name        | Description                                                                     |
|---------------------------------------|-------------------|---------------------------------------------------------------------------------|
| Common Access Log                     | access_log        | The default web access log format for servers like Apache.                      |
| Amazon ALB log                        | alb_log           | Log format for Amazon Application Load Balancers                                |
| VMware vSphere Auto Deploy log format | autodeploy_log    | The log format for the VMware Auto Deploy service                               |
| Generic Block                         | block_log         | A generic format for logs, like cron, that have a date at the start of a block. |
| Candlepin log format                  | candlepin_log     | Log format used by Candlepin registration system                                |
| Yum choose_repo Log                   | choose_repo_log   | The log format for the yum choose_repo tool.                                    |
| CUPS log format                       | cups_log          | Log format used by the Common Unix Printing System                              |
| Dpkg Log                              | dpkg_log          | The debian dpkg log.                                                            |
| Amazon ELB log                        | elb_log           | Log format for Amazon Elastic Load Balancers                                    |
| engine log                            | engine_log        | The log format for the engine.log files from RHEV/oVirt                         |
| Common Error Log                      | error_log         | The default web error log format for servers like Apache.                       |
| Fsck_hfs Log                          | fsck_hfs_log      | Log for the fsck_hfs tool on Mac OS X.                                          |
| Glog                                  | glog_log          | The google glog format.                                                         |
| HAProxy HTTP Log Format               | haproxy_log       | The HAProxy log format                                                          |
| Java log format                       | java_log          | Log format used by log4j and output by most java programs                       |
| journalctl JSON log format            | journald_json_log | Logger format as created by systemd journalctl -o json                          |
| Katello log format                    | katello_log       | Log format used by katello and foreman as used in Satellite 6.                  |
| OpenAM Log                            | openam_log        | The OpenAM identity provider.                                                   |
| OpenAM Debug Log                      | openamdb_log      | Debug logs for the OpenAM identity provider.                                    |
| OpenStack log format                  | openstack_log     | The log format for the OpenStack log files                                      |
| CUPS Page Log                         | page_log          | The CUPS server log of printed pages.                                           |
| Papertrail Service                    | papertrail_log    | Log format for the papertrail log management service                            |
| S3 Access Log                         | s3_log            | S3 server access log format                                                     |
| SnapLogic Server Log                  | snaplogic_log     | The SnapLogic server log format.                                                |
| SSSD log format                       | sssd_log          | Log format used by the System Security Services Daemon                          |
| Strace                                | strace_log        | The strace output format.                                                       |
| sudo                                  | sudo_log          | The sudo privilege management tool.                                             |
| Syslog                                | syslog_log        | The system logger format found on most posix systems.                           |
| TCF Log                               | tcf_log           | Target Communication Framework log                                              |
| TCSH History                          | tcsh_history      | The tcsh history file format.                                                   |
| Uwsgi Log                             | uwsgi_log         | The uwsgi log format.                                                           |
| Vdsm Logs                             | vdsm_log          | Vdsm log format                                                                 |
| VMKernel Logs                         | vmk_log           | The VMKernel’s log format                                                       |
| VMware Logs                           | vmw_log           | One of the log formats used in VMware’s ESXi and vCenter software.              |
| RHN server XMLRPC log format          | xmlrpc_log        | Generated by Satellite’s XMLRPC component                                       |

If you have logs that are not automatically supported in lnav, like logs from an application that you wrote yourself, you can define a format for that using a json config file.<br>
As this is a whole topic in itself, this tutorial won't cover that process, but it is described in detail [here](https://docs.lnav.org/en/latest/formats.html).
