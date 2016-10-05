# django-gulp-nginx

[![Build Status](https://travis-ci.org/chouseknecht/django-gulp-nginx.svg?branch=master)](https://travis-ci.org/chouseknecht/django-gulp-nginx)

Simple Django web application to demo [Ansible Container](https://github.com/ansible/ansible-container).

Ansible Container makes it possible to build container images using Ansible Playbooks rather than Dockerfile, and
provides the tools you need to manage the complete container lifecycle from development to deployment.

With Ansible Container you get: 

- Tools you already know: Ansible and Docker Compose
- Highly reusable code by way of Ansible roles
- Easy to read and understand image build instructions contained in an playbook
- Repeatable and testable image build process
- A single orchestration document with settings for development and production
- Auto-generated deployment role and playbook  

## Requirements

[Ansible Container](https://github.com/ansible/ansible-container)

Ansible Container requires access to a running Docker Engine or Docker Machine. For help with the installation, see
our [installation guide](http://docs.ansible.com/ansible-container/installation.html).


## Usage

To run this app locally, create a project directory, and initialize it using Ansible Container. Pass the name of this
project to the `init` command, and you'll instantly have a ready-to-go application:

```
$ mkdir demo
$ cd demo
$ ansible-container init chouseknecht.django-gulp-nginx 
```

Now from your project directory build the images:

```
$ ansible-container build
```

And finally, from your project directory run the app:

```
$ ansible-container run
```
 
