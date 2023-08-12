# AWS-Dynatrace-CloudResumeChallenge

![2023-08-08 18_08_30-Window](https://github.com/SchmaltzVisuals/AWS-Dynatrace-CloudResumeChallenge/assets/38481385/d83da08f-7568-41c5-ba2a-8540a6c9cdee)

The CloudResumeChallenge was fun to go through and helped me gain practical AWS use. I put a twist on this challenge by integrating Dynatrace for synthetic monitoring of my website https://lnkd.in/gjh4r78V. This is one of the many projects I'll complete as I work moving into a cloud-focused/site-reliability role.

Overall the challenge involved:
1. Setting up a hosted zone through 53
2. Routing traffic to CloudFront
3. Enabling SSL/TLS with Certificate Manager (enables an encrypted connection to my website)
4. Storing my website files in an S3 Bucket
5. CloudFront is linked to my Bucket in order to display the website.
6. Lambda is used for triggering the event of incrementing website view count in DynamoDB every time my site is visiting (when a user navigates to https://lnkd.in/gjh4r78V, a JS function is run automatically which triggers my lambda function
7. To enable CI/CD I used GitHub with AWS CodePipeline

The final steps included monitoring my domain with synthetic traffic and monitoring CloudFront for errors and general statistics with CloudWatch.

AWS Technology used:
- CloudFront
- CloudWatch
- S3
- Lambda
- DynamoDB
- Route 53
- CodePipeline
- Certificate Manager

External:
- GitHub
- Dynatrace
- HTML, CSS, JavaScript, React, and Node.js for my website

The delay for synthetic events from Sydney Australia is due to my CloudFront distribution only being hosted in North America and Europe as this is the cheapest option. Utilizing AWS edge locations would solve the delay but is the highest price class.

Overall, this was a great "practical use case" project.
