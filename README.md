# slack_notify_tekton
used to send slack message using webhook details

This is the simple task to send message to slack using webhook details.

Step 1:-
Run the below command to install that uses slack-webhook details.
kubectl apply -f https://raw.githubusercontent.com/tektoncd/catalog/v1beta1/slackmessage/send-to-webhook-slack.yaml

Step 2: 
Create the secret file which contains the webhook URL of your team channel.

execute the below command 
kubectl apply -f webhook-secret.yaml

Step 3: -
Task run.

tkn task start send-slack-webhook.

Later it will show the command to check the log details of the taskrun.
