Our end-of-second-year project at INSAT codenamed Kli8nt, is a revolutionary platform that streamlines the process of deploying applications and databases on Kubernetes clusters. Our user-friendly interface allows users to authenticate to GitHub, select a repository, specify the stack, run and build commands, and deploy with ease.

Our backend server, written in Go, leverages the GitHub deployment API to clone repositories, use templates for stacks, add environment variables, and build and push images to our private container registry. We've also developed a custom Kubernetes operator that manages custom resource definitions (CRDs), automating application and database deployment and exposing them using Kubernetes services, with ingress rules behind the Nginx ingress operator.

To ensure seamless communication between the backend and Kubernetes, we use Redis as our messaging system. Additionally, we've integrated Cloudflare API to generate user subdomains on kli8nt.xyz when deployment is complete. We monitor the infrastructure with Prometheus and Grafana.

We use Google Cloud's Kubernetes Engine, Compute Engine for backend, and App Engine for the React TypeScript frontend. Our production deployment environment generates a webhook for future pushes (to trigger our backend) and displays the deployment URL upon success.

Plan:

![](plan.png)

Roadmap:

- We will need to make a custom K8s controller/operator based on Client-go
- Integrate Redis into the backend for communications with Kubernetes Cluster.
- Implement logging, alerting, and monitoring using Prometheus.
- Allocate sub-domains using Cloudflare API and configure Nginx ingress controllers for load balancing and routing web traffic to MSAs.
- Establish a CLI utility as well as a frontend interface for communications with end-user.

More specifics will be added as we go through the project!

This is the start of the TODO as usual, but we're currently in the research phase!

- [ ] Placeholder - not yet done
- [x] Placeholder - done!

- [x] Accessing end-user repos including private and the auth token in order to clone private repos `git clone https://oauth2:ghp_...Gnm61dm4rh@github.com/gituser/testrepo.git`
- [ ] Showing the production environment on the end user github repo just like github pages and vercel
- [ ] Making a front end interface to interact with the github-oauth2 backend

Follow up if you are interested! We'll be happy about it!
Thanks!
