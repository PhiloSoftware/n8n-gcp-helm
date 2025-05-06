# N8N Helm Chart for Google Kubernetes Engine
Simple Helm chart to stand up N8N in Google Kubernetes Engine using a managed Postgres DB using
Google's Cloud Sql Proxy.

I also use Traefik as a proxy so this creates an IngressRoute for that. 

I initially tried rolling out using https://github.com/8gears/n8n-helm-chart but I could not 
get that helm chart to connect to the Postgres DB.

So I took the yaml files from https://github.com/n8n-io/n8n-kubernetes-hosting and set up my
DB loaded as a sidecar to the primary N8N container. 


Feel free to use as required.