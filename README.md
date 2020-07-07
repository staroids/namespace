# Deploy an empty Kubernetes namespace

Deploys an empty Kubernetes namespace in Staroid.

![](https://user-images.githubusercontent.com/1540981/86824681-533bef00-c043-11ea-9911-de6b736d0380.gif)

Once deployed, you can create a shell from your browser and use `kubectl` command to play around.

[![Run](https://staroid.com/api/run/button.svg)](https://staroid.com/api/run)

## Ingress configuration

Creating a Service object with name 'staroid-service' with port 8080. Ingress will automatically configured to the service and `Open` button on the screen will open a browser to the address.

By default, ingress requires authentication and permission to access your Kubernetes cluster instance.

To allow public access, click "Public access" switch on the screen.

![](https://user-images.githubusercontent.com/1540981/86825864-c134e600-c044-11ea-9fee-66c10cbb8a55.png)

## Link to Service

You can show a link on the screen to connect any Service, by adding `service.staroid.com/link: "show"` annotation.
See https://docs.staroid.com/references/resources.html#service

Note that the Service not configured to the ingress always require authentication even if "Public access" switch is on.

## Supported Kubernetes resources

See https://docs.staroid.com/references/resources.html 
