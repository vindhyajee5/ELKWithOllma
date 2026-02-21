Steps1: namespace.yaml
C:\Users\vindh\OneDrive\Desktop\ai-log-analyzer>kubectl apply -f namespace.yaml
namespace/ai-logs created

Step2:-ELK

C:\Users\vindh\OneDrive\Desktop\ai-log-analyzer>kubectl apply -f elasticsearch.yaml
deployment.apps/elasticsearch created
service/elasticsearch created

C:\Users\vindh\OneDrive\Desktop\ai-log-analyzer>kubectl apply -f logstash.yaml
configmap/logstash-config created
deployment.apps/logstash created
service/logstash created

C:\Users\vindh\OneDrive\Desktop\ai-log-analyzer>kubectl apply -f kibana.yaml
deployment.apps/kibana created
service/kibana created

 

Kibana UI : http://localhost:30001
 
 



🔹 Step 1: Click “Explore on my own”
On your screen you see:
Start by adding integrations
[Add integrations] [Explore on my own]
👉 Click “Explore on my own”
________________________________________
🔹 Step 2: Go to Stack Management
On the left sidebar:
1.	Click ☰ (Menu icon)
2.	Click Stack Management

 

Step 3: Open Index Patterns / Data Views
Inside Stack Management:
1.	Click Data Views
(In older versions it is called Index Patterns)
 

C:\Users\vindh\OneDrive\Desktop\ai-log-analyzer>kubectl apply -f dummy-logger.yaml
pod/dummy-logger created

 

 

OLLAMA setup:-
 


STEP 6 — Verify Everything
Check pods:
kubectl get pods -n ai-logs
Check jobs:
kubectl get jobs -n ai-logs
Check analyzer logs:
kubectl logs <job-pod-name> -n ai-logs
You should see:
Latest Log: NullPointerException at OrderService.java:45

AI Response:
Root cause likely null object reference...


Summary :All File there  

This for all yaml  as per below github:
