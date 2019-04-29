# C2S for Red Hat Enterprise Linux 7

[![Build Status](https://travis-ci.org/RedHatOfficial/ansible-role-rhel7-c2s.svg?branch=master)](https://travis-ci.org/RedHatOfficial/ansible-role-rhel7-c2s)
[![Ansible Role](https://img.shields.io/ansible/role/29989.svg)](https://galaxy.ansible.com/RedHatOfficial/rhel7_c2s)
[![GitHub release](https://img.shields.io/github/release/RedHatOfficial/ansible-role-rhel7-c2s.svg)](https://github.com/RedHatOfficial/ansible-role-rhel7-c2s/releases/latest)

Ansible Role for C2S for Red Hat Enterprise Linux 7

Profile Description:  
This profile demonstrates compliance against the  
U.S. Government Commercial Cloud Services (C2S) baseline.  
  
This baseline was inspired by the Center for Internet Security  
(CIS) Red Hat Enterprise Linux 7 Benchmark, v2.1.1 - 01-31-2017.  
  
For the SCAP Security Guide project to remain in compliance with  
CIS' terms and conditions, specifically Restrictions(8), note  
there is no representation or claim that the C2S profile will  
ensure a system is in compliance or consistency with the CIS  
baseline.

The tasks that are used in this role are generated using OpenSCAP.
See the OpenSCAP project for more details on Ansible playbook generation at [https://github.com/OpenSCAP/openscap](https://github.com/OpenSCAP/openscap)

To submit a fix or enhancement for an Ansible task that is failing or missing,
see the ComplianceAsCode project at [https://github.com/ComplianceAsCode/content](https://github.com/ComplianceAsCode/content)

## Requirements

- Ansible version 2.5 or higher

## Role Variables

To customize the role to your liking, check out the [list of variables](vars/main.yml).

## Dependencies

N/A

## Example Playbook

Run `ansible-galaxy install RedHatOfficial.rhel7_c2s` to
download and install the role. Then, you can use the following playbook snippet to run the Ansible role:

    - hosts: all
      roles:
         - { role: RedHatOfficial.rhel7_c2s }

Next, check the playbook using (on the localhost) the following example:

    ansible-playbook -i "localhost," -c local --check playbook.yml

To deploy it, use (this may change configuration of your local machine!):

    ansible-playbook -i "localhost," -c local playbook.yml


## License

BSD-3-Clause

## Author Information

This Ansible remediation role has been generated from the body of security
policies developed by the ComplianceAsCode project. Please see
[https://github.com/complianceascode/content/blob/master/Contributors.md](https://github.com/complianceascode/content/blob/master/Contributors.md)
for an updated list of authors and contributors.
