Step 1: Create a namespace for mointoring tool

           
           kubectl create namespace dynatrace
           
           
Step 2: Install helm package manager 
        
        sudo snap install helm --classic

Step 3: Add Dynatrace repo on your machine with this command

        helm repo add dynatrace https://raw.githubusercontent.com/Dynatrace/dynatrace-operator/main/config/helm/repos/stable
        

Step 4: And update your helm repo
         
         helm repo update
         
Step 5: Install the Dynatrace Operator
        * before Install the Dynatrace Operator we need Environment ID and API Token
        * we can get environment ID with URL and Account Management > Settings > Environments ID
        * To get API token to see Access Token section you can see the token you generated
        * Intsall command for Dynatrace Operator

        helm install dynatrace-operator dynatrace/dynatrace-operator --namespace dynatrace --set platform=kubernetes --set apiServer="https://hho46211.live.dynatrace.com/api" --set apiToken="dt0c01.6OSHFEZURGPB655CYJJ4GDAU" --set skipCertCheck=false --create-namespace

Step 6: 
  
