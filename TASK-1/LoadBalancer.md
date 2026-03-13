# Create vpc 
1. click on serch tab serch vpc
2. click on vpc icone
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/28a7bb12-6642-4dd5-bb1f-defb4e3f6e6c" />
3. click on create VPC
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/d15db2de-8aea-41de-999b-44644173dee7" />
4. Resources to create me choice *VPC Only*
5. Name tag Type *Project-VPC*
6. IPv4 CIDR Type *10.0.0.0/24*
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/9ed6ba67-95fa-47a3-b279-bdd731d17536" />
7. click on Create VPC
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/e2c3cf09-9002-430a-a832-159164919153" />

# create Subnet
1. click on Subnet
<img width="1919" height="1073" alt="image" src="https://github.com/user-attachments/assets/c2bebdf9-d30b-4619-82ea-dca794da5899" />
2. click on create subnet
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/ea8b5121-33ad-4acb-9d04-79c95d64de9c" />
3. select VPC ID *Project-VPC*
<img width="1919" height="1073" alt="image" src="https://github.com/user-attachments/assets/a0b5230e-54ef-406a-add6-38fe2fb92ee0" />
4.Go to Subnet Setting
5. Subnet 1
   1. Subnet name *Public-Sub-1*
   2. Availability Zone * (ap-south-1a)*
   3. IPv4 subnet CIDR block *10.0.1.0/24*
   4. click on add new subnet
<img width="1919" height="1077" alt="image" src="https://github.com/user-attachments/assets/630eb038-b5e0-4fb7-bb7e-6456741fb533" />
 6. Subnet 2
   1. Subnet name *Public-Sub-2*
   2. Availability Zone * (ap-south-1b)*
   3. IPv4 subnet CIDR block *10.0.2.0/24*
   4. click on add new subnet
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/b70e30d6-647e-449b-9c07-05a55c59633a" />
7. Subnet 3
   1. Subnet name *Private-Sub-1*
   2. Availability Zone * (ap-south-1a)*
   3. IPv4 subnet CIDR block *10.0.3.0/24*
   4. click on add new subnet
<img width="1919" height="1077" alt="image" src="https://github.com/user-attachments/assets/9095d2b7-f1d0-4e06-9160-1b1ac604b863" />
8. Subnet 4
   1. Subnet name *Private-Sub-2*
   2. Availability Zone * (ap-south-1b)*
   3. IPv4 subnet CIDR block *10.0.4.0/24*
   4. click on Create Subnet
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/d7f10966-8691-4a40-87e8-c7c02014a808" />
9. Now you caan see All subnets
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/d1b7aa2c-b751-4996-abc1-d5eb4ff9f05c" />

# Internet Gateway 
1. Click On imternet Gateway
2. click on Create Internet Gateway
<img width="1919" height="1079" alt="Screenshot 2026-03-13 104732" src="https://github.com/user-attachments/assets/e7ded44e-f9de-4708-99e2-da02bd71dbe6" />
3. InterNagetway setting
4. Give name *Project-IGW*
5. click on Create Internet Gateway
<img width="1919" height="1075" alt="image" src="https://github.com/user-attachments/assets/98716cd5-f173-4eb3-80b2-51681a177bfb" />
6. click on Action
7. click on atach to Vpc
<img width="1919" height="1075" alt="image" src="https://github.com/user-attachments/assets/a063deee-054f-4e41-b906-a9873d3a22b5" />
8. click on Avalable Vpc
9. select *Projrct-VPC*
10. click on Attach Internet Gateway
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/84a7ced0-abd2-454f-abda-1f6c55d7d894" />

# Create Nat Gateway
1. click on Nat Gateway
2. click on Create Nat Gateway
<img width="1919" height="1073" alt="image" src="https://github.com/user-attachments/assets/2aa2b7c0-5c3e-4d26-b56e-cf1e3ad3c7fb" />
3. Nat Gateway Setting
4. Type Name *Project-Nat*
5. Select Avability Mode *Rigional*
6. select VPC *Project-VPC*
7. Method of Elastic IP (EIP) allocation *Atomaticaly*
8. click on Create NAt Gateway
<img width="1919" height="1075" alt="image" src="https://github.com/user-attachments/assets/07075cc9-2a6d-4264-bd14-d54ce9cfb8ff" />


# create Route Table 
## Public Route Table
1. we can create vpc so atomaticaly 1 route table is created
2. click on Route table
3. Edit Name *Public-Route-Table*
4. click on Save
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/12bed074-85c3-4cff-aee9-f1368fbe1d3d" />
### Route Edit
5. select Public-Route-Table
7. click on Routes
8. click On edite Routes
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/65f62c15-e62d-4af6-b693-f3382a80612d" />
9. Select Destination *0.0.0.0/0*
10. select Target *InternetGateway* -----> *Project-IGW*
11. click On save Chenges
<img width="1918" height="1076" alt="image" src="https://github.com/user-attachments/assets/05311e23-25b0-4ea7-80a3-5b554090e8c4" />
### Subnet Asociate  
1. click On Subnet Asoosiate
2. click on Edit subnet Assosiate
<img width="1919" height="1072" alt="image" src="https://github.com/user-attachments/assets/6cf8364f-31aa-449c-96bf-a85453be4496" />
3. select avalable Subnet
   1. Public-Sub-1
   2. Public-Sub-2
4. click on save asociate
<img width="1919" height="1075" alt="image" src="https://github.com/user-attachments/assets/42448600-b7c7-46bf-9bc3-bd88c82b5969" />

## Private Route Table
1. click on Route Table
2. click on Create Route Table 
<img width="1919" height="1073" alt="image" src="https://github.com/user-attachments/assets/07678fa2-28a7-48b2-a95c-1522aa6483de" />
3. Route table settings
4. Name *Private Route-Table*
5. select vpc *Project-VPC*
6. click on Create Route Table
<img width="1919" height="1074" alt="image" src="https://github.com/user-attachments/assets/b284c9bb-1c50-4462-97ed-8848579fc6d7" />

### Route Edit
1. click on Routes
2. click on Edit Routes
<img width="1919" height="1074" alt="image" src="https://github.com/user-attachments/assets/a7686c20-6b3f-45df-8cb6-aa07b257f961" />
3. click on Add routes
3. Destination *0.0.0.0/0*
4. Target *NAT Gateway* ------> *Project-NAt*
5. click on save
<img width="1919" height="1072" alt="image" src="https://github.com/user-attachments/assets/782cfcce-2a51-4517-81ae-61d78175f696" />

### Subnet Asociate  
1. click on Subnet Assosiate
2. click on Edit Subnet Assosiate
<img width="1919" height="1078" alt="image" src="https://github.com/user-attachments/assets/b1bd6a83-2804-467b-a160-8e11314f0ee2" />
3. avalable Subnet
   1. Private-sub-1
   2. private-sub-2
4. save Association
<img width="1919" height="1074" alt="image" src="https://github.com/user-attachments/assets/6a99e23e-bdad-4fbc-86c4-34ef5808f0c2" />


# Create Ec2 FrontEnd/Basion on public Subnet
1. go to Ec2 Dashbord
2. click on Instance
3. click on Lonch Enstance
<img width="1919" height="1072" alt="image" src="https://github.com/user-attachments/assets/6ab21f0c-e3fe-4d93-8ba8-2e39cbf1e713" />
4. Launch an instance
   1. Name: *Bastion/FronEnd*
   2. Application and OS Images (Amazon Machine Image) : *Ubuntu*
   <img width="1919" height="1075" alt="image" src="https://github.com/user-attachments/assets/3a0a159c-c313-431a-8cd4-541835544fac" />

   4. Instance type : *t3micro*
   5. key pair : *MumbaiKey*
   <img width="1919" height="1076" alt="image" src="https://github.com/user-attachments/assets/1c891081-dc54-4743-ac41-d2c4e489184e" />

   7. Network setting : *Edit*
      1. VPC Choice : *Project-VPC*
      2. Subnet choice : *Public-Sub-1*
      3. Auto-assign public IP : *Anable*
      4. Security Group Name : *Public-Security-Group*
      5. click on Lonch Enstance
      <img width="1919" height="1075" alt="image" src="https://github.com/user-attachments/assets/f7a2b8b8-7336-4909-9674-b8b949c529b0" />

## Security Group
1. select Bation FrontEnd enstance
2. click on sucurity Tab
3. click on security Group Id
<img width="1919" height="1077" alt="image" src="https://github.com/user-attachments/assets/a99a7b07-477d-442f-acf6-32be7ab86ab9" />
3. click on Edit Enbound Rule
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/61fdad35-3322-408b-8fc4-6fe4d3ee8e00" />
4. click on Add Rule
5. type : *All Trafic*
6. cource : *Anywhere*
7. click on Save Rule
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/3c8a7b67-f808-4d3e-b9d2-19d8e476dadb" />


## Conect Basion/Frondend Ec2
1. Swich to root user : `sudo su - `
2. create file `vi FrontEnd.sh`
3. Paste the shall sript Here the link `https://github.com/PRATHAMKUKUDKAR/AWS/blob/main/TASKS/TASK-1/Scripts/FrontEnd/FrontEnd.sh`
4. Give permission : ` chmood 777 FrontEnd.sh`
5. Run The Sripts : `./FrontEnd.sh`
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/48ef5848-1caa-4cb0-9cc7-dc525c229774" />

# Create EC2 Backent on Private Subnet 1
`Train-1`
`Bus-1`
`Flight-1`
1. click On Instance
2. click on Launch Instance
<img width="1907" height="1076" alt="image" src="https://github.com/user-attachments/assets/edf468d9-7c1d-4b80-856f-e084d0330c04" />
3. name : *Train-1*
4. select Application and OS Images (Amazon Machine Image) : *Ubuntu*
5. Number of instances : `3`
<img width="1919" height="1073" alt="image" src="https://github.com/user-attachments/assets/382f5ce9-31e1-472b-b9a5-9376997608d1" />

6. Instance type : *t3micro*
7. key pair : *MumbaiKey*
<img width="1919" height="1073" alt="image" src="https://github.com/user-attachments/assets/faee3d55-6f28-4acc-9926-e73cca66088b" />

8. Network setting : *Edit*
      1. VPC Choice : *Project-VPC*
      2. Subnet choice : *Private-Sub-1*
      3. Auto-assign public IP : *Disable*
      4. Security Group Name : *Private-Security-Group*
      5. click on Lonch Enstance
   <img width="1919" height="1073" alt="image" src="https://github.com/user-attachments/assets/dcd13ca4-7ede-4ebd-9d3b-6017471a483c" />
9. Reaname the Instance Name `Train-1` `Bus-1` `Flight-1`
<img width="1919" height="1076" alt="image" src="https://github.com/user-attachments/assets/bd923e6d-5520-4e97-9acc-266cdeec367f" />

## Security Group
1. select Train-1 enstance
2. click on sucurity Tab
3. click on security Group Id
<img width="1919" height="1076" alt="image" src="https://github.com/user-attachments/assets/4292781a-014c-4eb4-8924-2ad97f5147aa" />

3. click on Edit Enbound Rule
<img width="1919" height="1074" alt="image" src="https://github.com/user-attachments/assets/30ee3bf0-d89e-4d50-9871-4fddc7655a67" />

4. click on Add Rule
5. type : *All Trafic*
6. cource : *Anywhere*
7. click on Save Rule
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/c07c0793-404a-4404-a1bc-bd3cb47ce43e" />

## Conect Ec2 Train-1
1. first login BastionHost
2. create Pem file `vi MumbaiKey.pem`
3. give permission : `chmod 400 MumbaiKey.pem`
4. connect to Train-1 enstance : `ssh -i "MumbaiKey.pem" ubuntu@10.0.3.100`
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/a23d304d-07af-4e62-98c6-1a3cc89acd93" />

5. create file `vi Train-1.sh`
6. Paste the shall sript : Here the Link `https://github.com/PRATHAMKUKUDKAR/AWS/blob/main/TASKS/TASK-1/Scripts/Train/Train-1.sh`
7. Give permission : ` chmood 777 Train-1.sh`
8. Run The Sripts : `./Train-1.sh`
<img width="1915" height="1079" alt="image" src="https://github.com/user-attachments/assets/6aaf564e-b6ef-4ff0-bb19-d722fb664557" />

## Conect Ec2 Bus-1
1. first login BastionHost
2. Connect to Bus-1 Enstance : `ssh -i "MumbaiKey.pem" ubuntu@10.0.3.101`
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/3127e53f-528e-4d98-ac42-36dadd9dc4c4" />

3. create file `vi Bus-1.sh`
4. Paste the shall sript Here the link `https://github.com/PRATHAMKUKUDKAR/AWS/blob/main/TASKS/TASK-1/Scripts/Bus/Bus-1.sh`
5. Give permission : ` chmood 777 Bus-1.sh`
6. Run The Sripts : `./Bus-1.sh`
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/d61def16-0fdc-477f-b688-bb3248cb8b41" />

## Conect Ec2 Flight-1
1. first login BastionHost
2. Connect to Flight-1 Enstance : `ssh -i "MumbaiKey.pem" ubuntu@10.0.3.101`
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/05b72244-d442-48bd-8978-f826b994afd5" />

3. create file `vi Flight-1.sh`
4. Paste the shall sript here the link `https://github.com/PRATHAMKUKUDKAR/AWS/blob/main/TASKS/TASK-1/Scripts/Flight/Flight-1.sh`
5. Give permission : ` chmood 777 Flight-1.sh`
6. Run The Sripts : `./Flight-1.sh`
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/8bde4f0b-93de-4782-aa34-061eabfc0fc8" />

# Create EC2 Backent on Private Subnet 2
`Train-2`
`Bus-2`
`Flight-2`
1. click On Instance
2. click on Launch Instance
<img width="1919" height="1078" alt="image" src="https://github.com/user-attachments/assets/652ba565-59bd-4ad7-97f9-0b5903c447b7" />

3. name : *Train-2*
4. select Application and OS Images (Amazon Machine Image) : *Ubuntu*
5. Number of instances : `3`
<img width="1918" height="1079" alt="image" src="https://github.com/user-attachments/assets/12c95f59-60ef-4797-a7c4-5daa0e17913c" />

6. Instance type : *t3micro*
7. key pair : *MumbaiKey*
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/6007a70a-52c5-492b-a67e-b5c041b08d14" />

8. Network setting : *Edit*
      1. VPC Choice : *Project-VPC*
      2. Subnet choice : *Private-Sub-2*
      3. Auto-assign public IP : *Disable*
      4. Select existing security group : *Private-Security-Group*
      5. click on Lonch Enstance
       <img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/798a4e00-9366-49c7-9a3e-d9bcba77c6c4" />

9. Reaname the Instance Name `Train-2` `Bus-2` `Flight-2`
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/aad6270d-bffe-4161-9bc1-829f3769fa68" />

## Conect Ec2 Train-2
1. first login BastionHost
2. Connect to Train-2 Enstance : `ssh -i "MumbaiKey.pem" ubuntu@10.0.3.101`
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/97a82e63-4bf8-4787-9550-aa4b872adb35" />

3. create file `vi Train-2.sh`
4. Paste the shall sript Here the link : `https://github.com/PRATHAMKUKUDKAR/AWS/blob/main/TASKS/TASK-1/Scripts/Train/Train-2.sh`
5. Give permission : ` chmood 777 Train-2.sh`
6. Run The Sripts : `./Train-2.sh`
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/2871af02-c51e-4fe5-ba5b-d71ecdcf05e6" />

## Conect Ec2 Bus-2
1. first login BastionHost
2. Connect to Bus-2 Enstance : `ssh -i "MumbaiKey.pem" ubuntu@10.0.3.101`
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/b7f1d745-f444-4cd4-be6c-11cf742cddd9" />

3. create file `vi Bus-2.sh`
4. Paste the shall sript Here the link : `https://github.com/PRATHAMKUKUDKAR/AWS/blob/main/TASKS/TASK-1/Scripts/Bus/Bus-2.sh`
5. Give permission : ` chmood 777 Bus-2.sh`
6. Run The Sripts : `./Bus-2.sh`
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/22ff88d5-458c-4944-88e4-ae34df6729af" />

## Conect Ec2 Flight-2
1. first login BastionHost
2. Connect to Flight-2 Enstance : `ssh -i "MumbaiKey.pem" ubuntu@10.0.3.101`
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/df6af4d5-a6e5-498a-99ba-eb382ef2870d" />

3. create file `vi Flight-2.sh`
4. Paste the shall sript here the link `https://github.com/PRATHAMKUKUDKAR/AWS/blob/main/TASKS/TASK-1/Scripts/Flight/Flight-2.sh`
5. Give permission : ` chmood 777 Flight-1.sh`
6. Run The Sripts : `./Flight-2.sh`
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/438e1862-664b-4026-8bf1-62d279b4004f" />
