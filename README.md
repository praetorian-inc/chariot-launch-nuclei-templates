# Overview

We've [developed twenty-three Nuclei templates](https://www.praetorian.com/blog/23-and-me-offensive-dna-and-nuclei-templates/) as part of the [launch of our attack surface management product offering](https://www.praetorian.com/blog/ides-of-march-chariots-launch-day/). The vast majority of these templates focus on detecting various web application services such as continuous integration and deployment systems as identifying opportunities to reduce external attack surfaces is a core part of the value proposition of our product offering. We've also developed some templates related to specific vulnerabilities (e.g. a remote code execution in the Code42 application using the Log4Shell vulnerability) and added support for token-spraying Fastly and Gitlab cloud.

## Continuous Integration and Deployment Applications:

* Ansible Semaphore (ansible-semaphore-panel.yaml): A user-interface leveraged to run Ansible playbooks (https://ansible-semaphore.com/)
* Buddy Enterprise (buddy-panel.yaml): A CI/CD application that can be deployed as a self-hosted solution (https://buddy.works/docs/on-premises/introduction)
* BuildBot (buildbot-panel.yaml): A continuous integration framework (https://buildbot.net/)
* Concouse CI (concourse-ci-panel.yaml): An open-source self-hosted continuous integration application (https://concourse-ci.org/)
* Drone CI/CD (drone-ci-panel): An open source continuous integration platform (https://www.drone.io/)
* Flow CI (flowci-detection.yaml): An open source continuous integration tool (https://flowci.github.io/#/)
* Strider CD (stridercd-detection.yaml): An open source continuous deployment application (https://strider-cd.github.io/)
*  Zuul CI (zuul-panel.yaml): An open source continuous integration tool (https://zuul-ci.org/)

## Enterprise Applications:

* Avatier Enterprise Password Management (avatier_password_management.yaml): Self-service portal that allows users to reset their password and unlock their accounts (https://www.avatier.com/products/identity-management/password-management/)
* Cofense Vision (cofense-vision-detection.yaml): Detection for management interface of Cofense Vision an appliance used to identify an quarantine phishing emails (https://cofense.com/project/cofense-vision/)
* Leostream (leostream-detection.yaml): Manages remote access through VDI (https://leostream.com/)
* Sophos Mobile Self Service Panel (sophos-mobile-panel-detection.yaml): Detection for the Sophos Mobile Self Service Portal (https://docs.sophos.com/esg/smc/9-6/admin/en-us/esg/Sophos-Mobile/concepts/ConfigureSSPAbout.html)
* Splunk Enterprise (splunk-enterprise-login-panel.yaml): Detection for the Splunk Enterprise application (https://www.splunk.com/en_us/software/splunk-enterprise.html)

## Other Applications
* Gradle Enterprise (gradle-enterprise-panel.yaml): A software build automation tool (https://gradle.com/)
* Gradle Enterprise Build Cache (gradle-enterprise-build-cache-detect.yaml): Build cache used by Gradle to save time by reusing outputs prodcued by other builds (https://docs.gradle.org/current/userguide/build_cache.html)
* HTTPBin (httpbin-detection): An application used to test HTTP client libraries (http://httpbin.org/)
* Redash (redash-detection.yaml): An application that is leveraged for visualizing data similar to Grafana (https://redash.io/)
* Zentral (zentral-detection.yaml): An open source event aggregator for osquery and Santa (Google's application allowlisting application) (https://zentral.io/)

## Exploits

* Code42 Log4j Exploit (log4j-code42-rce.yaml): Tests for the log4j vulnerability in the Code42 application
* HTTPBin Cross Site Scripting (httpbin-xss.yaml): Tests for an XSS issue present in the HTTPBin application
* HTTPBin Open Redirect (httpbin-open-redirect.yaml): Tests for an open redirection issue in the HTTPBin application

## Token Spraying:

* Gitlab Token Spraying (api-github.yaml): A new template for token spraying personal access tokens for the cloud version of Gitlab
* Fastly Token Spraying (api-fastly.yaml): A new template for token spraying the Fastly CDN provider to check if a given string is a valid Fastly API token.
