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


# Create Target Group 
## FrontEnd TG
1. click on Target Group
2. click Create Target Group
3. Setting:
   1. Target type : *Instance*
   2. Target group name : *FrontEnd-TG*
   3. Protocol : *HTTP*
   <img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/717263c7-dd7c-4c52-8cd8-5e3883ec67f0" />
   4. Selecct Vpc : *Project-VPC*
   <img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/7de21c5a-cac9-4925-9f7c-e53250aa15b5" />
   5. click on Next
   <img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/3d6196f1-1b54-4203-a868-0365bfdb453a" />

1. Select Enstance : `Bastion/FrontEnd`
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/a1b95042-9177-4d9a-9bfc-8dd71af13b96" />
2. click Include As pending Below
3. click Next
<img width="1919" height="1078" alt="image" src="https://github.com/user-attachments/assets/096fb088-95ec-4237-9194-be8a14304f38" />
4. Clock on Create Target Group
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/afea3ceb-11be-4d48-9bfa-24561898c49f" />



## Train-TG
2. click Create Target Group
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/ec462fc7-ea82-49e9-9a4b-91c2ada38604" />

4. Setting:
   1. Target type : *Instance*
   2. Target group name : *Train-TG*
   3. Protocol : *HTTP*
<img width="1919" height="1071" alt="image" src="https://github.com/user-attachments/assets/238fe9a7-1845-438d-ab81-9bb373fd2fd2" />
  
   4. Selecct Vpc : *Project-VPC*
   <img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/7de21c5a-cac9-4925-9f7c-e53250aa15b5" />
   5. click on Next
   <img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/3d6196f1-1b54-4203-a868-0365bfdb453a" />

1. Select Enstance : `Train-1` `Train-2`
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/d732128e-3b6b-450e-9c70-2fdfe898af96" />

2. click Include As pending Below
3. click Next
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/974f54c9-c864-45e7-a3bd-083f223d9bbd" />

4. Clock on Create Target Group
<img width="1919" height="1075" alt="image" src="https://github.com/user-attachments/assets/636a158b-54ab-42dd-b54a-ef4703907e9a" />


## Bus-TG
2. click Create Target Group
<img width="1919" height="1074" alt="image" src="https://github.com/user-attachments/assets/2e0e6192-b4f1-491a-88bc-26b56cf38eb9" />

3. Setting:
   1. Target type : *Instance*
   2. Target group name : *Bus-TG*
   3. Protocol : *HTTP*
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/d95b8db9-12d4-411b-be3e-07f3aad9dc9e" />

   4. Selecct Vpc : *Project-VPC*
 <img width="1919" height="1075" alt="image" src="https://github.com/user-attachments/assets/46f3f0e8-5d97-4212-806e-3dcdd6412e69" />

   5. click on Next
   <img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/ec2afac6-2592-4e2f-806f-19c5307d1673" />

1. Select Enstance : `Bus-1` `Bus-2`
<img width="1919" height="1073" alt="image" src="https://github.com/user-attachments/assets/ae370a21-b53e-4cd9-b3c0-95a75fea3bd5" />

2. click Include As pending Below
3. click Next
<img width="1919" height="1074" alt="image" src="https://github.com/user-attachments/assets/3fd837e3-ac6d-45e1-9736-b4618810a2c8" />

4. Clock on Create Target Group
<img width="1919" height="1078" alt="image" src="https://github.com/user-attachments/assets/8e870ff2-a4f8-412b-980b-241d19e278a1" />


## Flight-TG
2. click Create Target Group
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/16e3953f-966d-46e1-9fff-8f9c067c9316" />

3. Setting:
   1. Target type : *Instance*
   2. Target group name : *Flight-TG*
   3. Protocol : *HTTP*
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/6ef9bfab-b105-4a6e-a3f4-28174cd0ca35" />

   4. Selecct Vpc : *Project-VPC*
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/8ddf3f12-dab6-47fb-9344-4dd735207acc" />

   5. click on Next
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/d415916f-f3d6-4ed7-91c8-5e8ec458f483" />

1. Select Enstance : `Flight-1` `Flight-2`
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/7c5d0a3f-fb6e-41eb-a7e1-a6ba008c21f1" />

2. click Include As pending Below
3. click Next
<img width="1919" height="1076" alt="image" src="https://github.com/user-attachments/assets/f25dee70-c805-466a-9cde-38559d64510f" />

4. Clock on Create Target Group
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/b832d4f7-769f-4b5a-9ba0-26cf05bcb9e1" />




# Create Load Balancer
1. click on Load BAlancer
2. click on Create LadBalance
<img width="1919" height="1075" alt="image" src="https://github.com/user-attachments/assets/fc8bd5c4-ef3c-4d87-be55-0839abb44367" />
3. Choice Aplication Load Balancer
4. click on Create
<img width="1919" height="1077" alt="image" src="https://github.com/user-attachments/assets/01899c68-4fa4-456f-946e-4b2c787b9874" />
5. Basic configuration
   1. Load balancer name : *Project-LB*
   2. Scheme : *Internet-facing*
   <img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/d1fb9743-29f8-4c81-9cc1-b17b972259d8" />

6. Network mapping
   1. Select Vpc : *Project-VPC
   2. select Avability Zone And Subnet : (1) *ap-south-1a * *Public-Sub-1* (2) *ap-south-1b * *Public-Sub-2*
<img width="1888" height="1067" alt="image" src="https://github.com/user-attachments/assets/f71e5be3-357b-4b50-a4a2-1043dc48013a" />

7. Listeners and routing
   1. Routing action : *Forward to target groups*
   2. Select Target group : *FrontEnd* 

8. Click On Create LOad Balancer
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/c8667116-8bbc-418e-9a63-245d872c30e5" />

9. click on Add Lisner
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/40244ddd-79a1-4928-8feb-45e7cb68ac4c" />

## Create Lisners And Rule
## Train-TG
1. Click On LIsners And Rules
2. click On HTTP:80
3. click on managerule
4. click on Add Rule
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/3dd9020a-cffa-4eb7-962d-513eae5a2da0" />
5. click on Codition
6. choice Path
7. Path condition value : */train* *
<img width="1887" height="1077" alt="image" src="https://github.com/user-attachments/assets/a58b810c-3020-4427-9f5c-7a422576e85a" />
8. Routing action : *Forward to target groups*
9. Select Target group : *Train-TG*
10. click on Next
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/8ed17229-0e70-4c90-8519-477bcbd0fe83" />

11. Type Priority : *1*
12. click on Next
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/b6caf2ad-3312-4d49-915a-ddcda60ca291" />
13. click on Add rule

<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/c1e4e1c3-2e2f-478a-9731-87262bbf71bf" />

## Bus-TG
1. click on Add Rule
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/eacf0de4-726c-41c8-b679-cd7dc4a79c06" />
2. click on Codition
3. choice Path
4. Path condition value : */bus* *
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/3aed3b02-ada2-4cfa-a8db-a8b555c4fe16" />
5. Routing action : *Forward to target groups*
6. Select Target group : *Bus-TG*
7. click on Next
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/6d8fe5e6-9e92-4a40-98e1-944628c94068" />
8. Type Priority : *2*
9. click on Next
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/d178bdca-b7d6-43d9-b1bb-569fff83072b" />
10. click on Add rule
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/60a431eb-b4eb-4fb2-8bb3-d4476915528d" />


## Flight-TG
1. click on Add Rule
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/f950f102-6225-4c0e-8eca-447976b01f93" />
2. click on Codition
3. choice Path
4. Path condition value : */flight* *
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/9eeb3507-94aa-4c81-8ce6-0766edaa4534" />
5. Routing action : *Forward to target groups*
6. Select Target group : *Flight-TG*
7. click on Next
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/ebff26b2-c3fe-4ede-b8e3-53accf544520" />

8. Type Priority : *3*
9. click on Next
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/0e15e9a3-3c5e-49d8-aac5-7cebd8f92b43" />

10. click on Add rule
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/dde62d4f-4958-40ed-b9c8-14a93003e6bc" />
