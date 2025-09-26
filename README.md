# Windows Firewall Rule Setup

## Objective
Configuring and testing basic firewall rules to block Telnet (port 23) on Windows.

## Steps Followed
1. **Listed Existing Rules:** Started "Windows Defender Firewall with Advanced Security" and viewed current inbound rules.  
   ![Inbound Rules](screenshots/rule-list.jpg)

2. **Created New Rule:**  
   - Selected 'Port' rule type. ![Rule Type](screenshots/rule-type.jpg)
   - Chose TCP, specified port 23. ![Protocol Ports](screenshots/protocol-port.jpg)
   - Selected 'Block the connection' action. ![Block Action](screenshots/block-action.jpg)
   - Named the rule 'Block Telnet'. ![Rule Name](screenshots/block-telnet.jpg)

3. **Tested the Rule:**  
   - Ran `telnet localhost 23` in command prompt to confirm:  
   ![Telnet Test](screenshots/telnet-test.jpg)  
   Output showed: "Could not open connection the host, on port 23: Connect failed".

4. **Firewall Status:**  
   - Checked firewall status and profiles. ![Firewall Status](screenshots/firewall-status.jpg)

## Key Learnings
- Learned how to create, apply, and test inbound firewall rules for specific ports in Windows.
- Understood how firewalls filter network traffic at port level.

## Commands Used
See [`commands_used.txt`](commands_used.txt).

## Summary
This task demonstrated practical skills in configuring Windows Firewall rules and validating their effect, building my fundamental network security expertise.
