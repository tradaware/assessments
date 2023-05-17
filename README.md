# Tradaware Assessments

## PSR-15 Middleware

**Hypothesis** 

We have some code that authenticates a client by _Basic Authentication_. Some of our clients can not provide this 
authentication header. To service these clients we want some middleware to allow authentication via credentials via 
HTTP POST or GET. 

> Credentials must be defined by the parameters **username** and **password**.

**Assignment**

Create PSR-15 middleware that looks for the credentials within the post or get request and adds these as basic 
authentication to the server request.

**Goals**

* The credentials parameters are removed from the url.   
* Incomplete or missing authentication/credentials must return a Forbidden or Unauthorized response.

**Workflow**

Fork this project, create your solution and to share your code with us by making a pull request
(see https://docs.github.com/en/get-started/quickstart/contributing-to-projects) or download this and create your 
solution and share this in a zip file via email (without the vendor folder).

You're free to use open source packages (like 
[slimframework](https://www.slimframework.com/docs/v4/start/installation.html) for instance) to help you to create and 
test your middleware. If you do so, please keep these packages within your composer.json file. Also leave any tests or 
code snippets you used during development; We love to see how you came up with your solution. 

Happy programming and good luck.

**Background**

* [PSR-15](https://www.php-fig.org/psr/psr-15/)
* [Basic Authentication](https://datatracker.ietf.org/doc/html/rfc7617)

