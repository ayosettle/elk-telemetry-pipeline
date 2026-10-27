# Linux Post-Compromise Detection Lab

**Status: work in progress**

A home lab that watches a Linux server for what an attacker does after getting in with stolen SSH credentials, then measures how well the alarms work.

## Goal
Collect useful host logs (auditd), write detection rules (Sigma, mapped to MITRE ATT&CK), and measure for each rule how often it catches the simulated attack, how often it raises false alarms on normal admin work, and how it can be evaded.

## Current progress
- [x] Ubuntu Server 24.04 VM (VirtualBox)
- [x] auditd installed, with rules for identity files, sudo config, cron/systemd persistence, and command execution
- [ ] SIEM (Elasticsearch + Kibana) and log shipping
- [ ] Attack and normal-activity simulation scripts
- [ ] Sigma detection rules
- [ ] Measurement and coverage report

Results and evidence will be added only after they have actually been produced.