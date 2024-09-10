##This is a static HTML website designed to be hosted on a cloud service.

The static-website-cloudformation.yaml file contains a cloudformation template that will deploy all the infrastructure for this site to be fully functional.

The Github Actions pipeline.yaml file, if you populate all of the appropriate secrets for your AWS account and for some of the assets and such, *should* deploy the content here to the infrastructure created by the cloudformation. If you'd rather not, though, it's fairly trivial with the assets created above to drag and drop into the S3 bucket. Not the most elegant solution, but you could do it.


TODOs:
- [ ] Create a splash page to hold the URL
- [ ] Create a menu bar
- [ ] Create a footer
- [ ] The header and footer should be on each page
- [ ] Integrate 
- [ ] An Api-gateway to allow the 'contact' page to process emails, requests for donations, etc.
- [ ] Integrate Shopify (?) or another card processor to process donations
- [ ] I'd like to integrate all of the above CI/CD wise.
- Eventually I'm going to Blue/Green this pipeline, not because zero downtime deployments being that important to my vanity site, but more because I want to show what it looks like. 😀


[![Test and Deploy Pipeline](https://github.com/edwardmccormick/vanity-website/actions/workflows/pipeline.yaml/badge.svg)](https://github.com/edwardmccormick/vanity-website/actions/workflows/pipeline.yaml)
[![pages-build-deployment](https://github.com/edwardmccormick/vanity-website/actions/workflows/pages/pages-build-deployment/badge.svg?branch=main)](https://github.com/edwardmccormick/vanity-website/actions/workflows/pages/pages-build-deployment)