# Overview

## Quick Links

- Getting access
- Setting up the local development environment

## How does the website work?
The website is splitted into a few parts - the  and the . Both of which are hosted in the College server.

### 1. Main website
The [main website](https://wcr.univ.ox.ac.uk) is frontend only, written in the [React.js](https://react.dev) framework, which integrates HTML, CSS and Javascript in the most intuitive way.

### 2. Content Management System
The [content management system](https://wcr.univ.ox.ac.uk/strapi) (CMS) is a standalone full-stack website. The codebase is provided by Strapi (v4 community edition).

### 3. Database
The website also contain a [Postgresql](https://www.postgresql.org) database.

### 4. Connecting main website, CMS and database
Everything is connected by the [Nginx](https://nginx.org) proxy server.

### 5. SSL
The certificate for Secure Sockets Layer (SSL) connection (i.e. the `https://` connection is provided by the [Let's Encrypt](https://letsencrypt.org), a nonprofit Certificate Authority. They have implemented the `certbot` which provides (semi-)automated way for us to apply for a certificate.

!!! warning

    The certbot implementation is buggy, and we are looking for permanent solution. For now, you will have to manually update the certificate.

### Docker
Everything listed above could be built using [the Docker engine](https://www.docker.com). Therefore, the only thing you have to install for development is the Docker engine. Once this is installed, you can run suitable commands to install the remaining website parts for local development/production.


!!! warning

    We will [upgrade the content management system](https://strapi.io/five) during the Christmas vacation to version 5. We may also consider using [Typescript](https://www.typescriptlang.org) over Javascript. As a result the documentation may need to be updated.

