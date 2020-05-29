# Monorepo Code + Infrastructure
When working in a DevOps environment (aka you build it, you run it), I like to have everything I do in code. This project is some kind of a monorepo approach to use Docker for local development in PHP, JS, ...
For the infrastructure part, I like Ansible a lot. For developing Ansible Playbooks, I tend to use Vagrant rather then Docker, simply because I like to have a "real" machine to test my Playbooks against.

# Usage
You could come up with some pipelines using GitLab CI or any other CI/CD tool (Jenkins, circle-ci, etc)... to run tests against your Docker setup using PHPUnit, then run some tests on your Ansible Playbooks, then run your Playbooks against your "hardware" and last but not least deploy your code changes in the last step. All Code needed to develop, run, test and deploy your whole project.