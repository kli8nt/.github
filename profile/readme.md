This is the start of the end-of-second-year project journey at INSAT, codenamed KLI8NT; automating deployment of web apps from GitHub repositories to the cluster.

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
