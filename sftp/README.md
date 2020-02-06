# SFTP Micro Service on Kubernetes 
Secure File Transfer Protocol (SSH File Transfer Protocol) is a network protocol that provides file access, file transfer, and file management over any reliable data stream.Compared to the SCP protocol, which only allows file transfers, the SFTP protocol allows for a range of operations on remote files which make it more like a remote file system protocol. An SFTP client's extra capabilities include resuming interrupted transfers, directory listings, and remote file removal.

## Who should read this?
1. If you are setting up/planning to setup  an SFTP server on a kubernetes and want to expose it to your users for pulling the logs or stats of other application logs/data.
2. If you want to see which external load balncer best fit for your sftp application for your kubernetes enviornment.
3. If you want to use SFTP micro service to run on your kubernetes.
4. If you dont know how to setup and share volume mount to your sftp server.
 
## This Section contains
1. Deploy a sftp micro service on a kubernetes cluster  
2. Using Citrix VPX as Ingress Device 
3. Access the sftp application.
4. Verify using VPX stats.

## Deploy sftp micro service on a kubernetes cluster
As a first setp we are dploying the SFTP micro service on kubernetes. Please refer [here](/sftp.yaml) to see the SFTP application yaml.

  
