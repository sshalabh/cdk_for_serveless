<img width="512" alt="image" src="https://user-images.githubusercontent.com/77447247/154659986-5d957ad5-8c39-41c1-8194-e67617927798.png">
This is the architecture of the solution I will be building in the demo
On the left there is a web application, which will be hosted on s3 object storage
This application communicates via a REST api on API Gateway
Which in turn points to a serverless lambda function
This lambda function will pull tweets from Twitter’s search API
These tweets then get send in an API call to Amazon Comprehend where sentyment analysis is performered
The result of this analysis is then returned by the lambda, via api Gateway to the web app, where it is displayed.
