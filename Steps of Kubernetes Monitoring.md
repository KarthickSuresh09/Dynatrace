Step 1: Create a namespace for mointoring tool

           
           kubectl create namespace dynatrace
           
           
Step 2: Install helm package manager 
        
        sudo snap install helm --classic

Step 3: Add Dynatrace repo on your machine with this command
        ```helm repo add dynatrace https://raw.githubusercontent.com/Dynatrace/dynatrace-operator/main/config/helm/repos/stable
        ```

Step 4: And update your helm repo
         ```helm repo update```
         
