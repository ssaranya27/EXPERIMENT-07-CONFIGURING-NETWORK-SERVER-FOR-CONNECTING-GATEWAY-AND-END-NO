### EXPERIMENT -07 CONFIGURING NETWORK SERVER FOR CONNECTING GATEWAY AND END NODE 
### NAME : SARANYA S.
### REG NO: 212223220101
## Aim: 
To  configure the Network server and end device for transferring data on the network
## Components required: 
End node stm 32 development kit , Dragino LPS8, Network server 

## Theory :
When working with sensitive applications or files, saving progress on your local device is a start, but what if you lose access to your device? Network servers address this problem by hosting the files and programs most pertinent to the network and enabling access for consistent, real-time use. 

As a result, personnel or network clients can instantly access important data or tools while also facilitating collaboration between users. Multiple users can make changes to the same program or document for continued development over the course of a project. Via a secure login, remote users can connect to the home network.
![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/59db9b76-ddd5-4d6a-9075-8db233f5e479)


In the above graphic, the circle represents an organization network where a network server facilitates collaboration and file sharing between network clients (devices).

 The role of a network server, then, is to provide users with a set of services and access to resources on the network. These features include:

Permissioned access and log-ins for network users Gateway access to the Internet for an organization Centralized location for network resources  Shared access to devices on the network like a printer or a scanner Hosts multi-user apps like email servers, web applications, or CRM

## Procedure :

 1. login to the network server using login link  https://iot.saveetha.in/
 2. Click on the nework server as shown blow
    
 ![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/1bd434ca-1426-4102-8384-94473483543e)
 3. Click on the add gateway 
 
 ![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/47c2e08d-6598-4437-8b07-f213d6f3b8ac)
![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/e62ff028-99bc-485e-9808-fbb6e124f8b2)
![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/a2e3ae58-6402-49e8-8f96-679059c1842c)
4. Click on the lora options , lora - frequency plan 

5. Click on channels and create a new channel after which you can add a new end device
   
![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/1fb72be5-e48d-4cde-a329-0cfb0d29070f)

6. Add the attributes in the end device as  shown below 

 ![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/00bff30b-42fc-42d5-9540-285d270e41cb)
 
7.Using AT commands configure end device in serial port utility
AT Commands to set initially (Mandatory)
 AT+FDR // To do factory data reset
 AT+NJM=1 // To set OTAA mode
 AT+ADR=1 // To enable the ADR
 AT+TDC=600000 // To set the default sampling interval as 10 minutes
(Should not give below 5 minutes)
 AT+CLASS=C // To set class C
 AT+DEUI=XX XX XX XX XX XX XX XX // To set Device EUI key
 AT+APPEUI=XX XX XX XX XX XX XX XX // To set APP EUI key
 AT+APPEUI=XX XX XX XX XX XX XX XX XX XX XX XX XX XX XX XX //
To set APP Key
 ATZ // To take effective action on below settings (As like saving)


## OUTPUT 
1.login to the network server using login link  https://iot.saveetha.in/
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/d15089e3-c275-4f5e-b398-4c4806bd6282" />
DEVICE TYPE
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/66202244-3360-4762-b10a-aef66909593f" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/20ea5b78-5a83-4e9b-a671-509b1e253b1d" />

DEVICE
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/4d2ad916-5b55-4e9a-a458-deca603bfba0" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/e69deeaa-ffd2-47e6-9a22-a66bb994c397" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/2d75dbd8-deca-46f3-ad77-5fb536fe62d9" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/7e2df707-8424-463f-88fc-80fe64550c99" />

GATEWAY:
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/800595d8-cbcd-47ae-98a2-c28305d8dcab" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/08820ea9-b717-4e51-a0c0-05af6c137539" />

AT COMMANDS:

<img width="1920" height="1080" alt="Screenshot (167)" src="https://github.com/user-attachments/assets/eaa1e55d-01d5-4d30-8580-a12e27f374e0" />
<img width="1920" height="1080" alt="Screenshot (168)" src="https://github.com/user-attachments/assets/7e310419-e4f1-4bc0-92da-d1002855866c" />
<img width="1920" height="1080" alt="Screenshot (169)" src="https://github.com/user-attachments/assets/fd794d0c-2b24-4166-bb15-2da7cfcbb333" />
<img width="1920" height="1080" alt="Screenshot (170)" src="https://github.com/user-attachments/assets/59a0a53c-5876-44c2-867b-57304e15b0bc" />
<img width="1920" height="1080" alt="Screenshot (171)" src="https://github.com/user-attachments/assets/5f1e51c2-c7b7-421c-b7af-cebbb508bfe4" />
<img width="1920" height="1080" alt="Screenshot (181)" src="https://github.com/user-attachments/assets/63046070-f41a-4ef5-bae1-e34113799160" />
<img width="1920" height="1080" alt="Screenshot (182)" src="https://github.com/user-attachments/assets/6a87737f-a241-4f73-a71e-7d0d54af366b" />
<img width="1920" height="1080" alt="Screenshot (183)" src="https://github.com/user-attachments/assets/da0909dc-3343-46ea-ac67-c0422f4ef5bb" />
<img width="1920" height="1080" alt="Screenshot (184)" src="https://github.com/user-attachments/assets/3341e188-09a7-4733-83a7-13ba392f0ed8" />

## Result: 

  The Network server and end device for transferring data on the network has been accomplished.
