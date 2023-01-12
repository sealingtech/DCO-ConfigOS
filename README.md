# DCO-ConfigOS

Objective: To provide a automated way ( Ansible ) for stig implementation & continuous compliance. Each OS/Platform has a dedicated ansible role created. Instructions of each can be found in respective directory. Testing is done in the RMF workspace on ST-LAB.
 
### Tracker:
| STIG/SRG                 |Versions    |Status           | % complete |
|--------------------------|------------|-----------------|-----------|
|Windows 10                | v2r4       |started          |  |
|ESXI 6.7                  | v1r2       |In progress      |  50%|
|RHEL8/Rocky8              | v1r8       |In Progress      |  80%|
|-                         | -          |-                | - |
|-                         | -          |-                | - |
|-           | -       |-     | - |

---

## Updates

### RHEL/Rocky 8: 68 Rules Remaining  
- Bulk of unremedied rules are related to PAM and manipulating configuration file.
- Additonal rules related to /etc/fstab and mount point options , however this will vary if DISA profile is elected upon provisioning. 
( note: Rocky OS does not complete installation if a DISA profile is selected at start-up, mount point configs and partition scheme would have to planned into kickstart/automation piece if applicable or manually done )

### ESXI7:  43 of 75 rules automated
- sub-playbooks created.
- some rules require vCenter component which has not been provisioned yet.


### WINDOWS10: 
- Having difficulties finding like type and module/tasks for ansible to Windows options and attributes.

	
