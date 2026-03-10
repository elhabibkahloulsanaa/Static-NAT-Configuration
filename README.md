# Static-NAT-Configuration

This lab demonstrates how to configure Static NAT on a Cisco router.

## Topics covered:
- Inside and outside interfaces
- Static NAT configuration
- NAT verification commands

## Step 1 — Configure Interfaces
enable

configure terminal

interface g0/0

ip address 192.168.1.1 255.255.255.0

ip nat inside

no shutdown

exit

interface g0/1

ip address 200.1.1.1 255.255.255.0

ip nat outside

no shutdown

exit

## Step 2 — Configure Static NAT

ip nat inside source static 192.168.1.10 200.1.1.10

## Step 3 — Verification

show ip nat translations

show ip nat statistics

## MORE ABOUT ME ON LINKEDIN :    https://www.linkedin.com/in/sanaa-el-habib-kahloul/ 
## If someone nedd any help : elhabibkahloulsanaa@gmail.com 
