# installing-helm
Demo to Install Helm on Ubuntu 21.10

In this Demo, I will be installing Helm on Ubuntu 21.10, using Helm Package for Apt

Steps:

1. Download Helm from curl
 
   Command: curl https://baltocdn.com/helm/signing.asc | gpg --dearmor | sudo tee /usr/share/keyrings/helm.gpg > /dev/null
   
   ![Screenshot from 2023-02-16 15-20-25](https://user-images.githubusercontent.com/122020679/219330456-0c39b2ff-3a5b-498a-91f6-6874b82c2f8e.png)

2. Command: sudo apt-get install apt-transport-https --yes

   ![Screenshot from 2023-02-16 15-21-36](https://user-images.githubusercontent.com/122020679/219330949-16999821-7fb1-42f9-9f37-84b9e052226e.png)
   
3. Command: echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/helm.gpg] https://baltocdn.com/helm/stable/debian/ all main" | sudo tee /etc/apt/sources.list.d/helm-stable-debian.list

   ![Screenshot from 2023-02-16 15-23-36](https://user-images.githubusercontent.com/122020679/219331418-048c6305-4e88-4147-9e91-603e4d38a5b1.png)

4. Command: sudo apt-get update

   ![Screenshot from 2023-02-16 15-25-09](https://user-images.githubusercontent.com/122020679/219331771-48feca1f-bab6-4ca0-a865-c73a30054020.png)

5. Insatll helm

   Command: sudo apt-get install helm
   
   ![Screenshot from 2023-02-16 15-26-32](https://user-images.githubusercontent.com/122020679/219332097-919b5405-4980-491f-8ee3-32067bd94992.png)

