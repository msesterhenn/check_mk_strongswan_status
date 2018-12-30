# check_mk_strongswan_status

Shows changes in the amount of active SAs on a strongSwan deployment.
This check requires an rule which establishes a SSH connection to the target system and outputs <<<strongswan_ipsec_status>>> and the output of 'ipsec status'.

ssh root@$HOSTADDRESS$ 'echo "<<<strongswan_ipsec_status>>>" && ipsec status'