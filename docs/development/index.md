# Overview

## Quick Links

- [Basic access](basic_access.md)
- [Server access](server_access.md)
- Setting up the local development environment (Docker)
- Basic editing of pages (React 101)
- Strapi API
- [What needs to be done?](new_features.md)

## How does the website work?
The website is splitted into a few parts - all of which are hosted in the College server, running using Linux Ubuntu 22.0 LTS.

### 1. Main website
The [main website](https://wcr.univ.ox.ac.uk) is frontend only, written in the [React.js](https://react.dev) framework, which integrates HTML, CSS and Javascript in the most intuitive way.

### 2. Content Management System
The [content management system](https://wcr.univ.ox.ac.uk/strapi) (CMS) is a standalone full-stack website. The codebase is provided by [Strapi](https://strapi.io) (v4 community edition).

### 3. Database
The website also contain a [Postgresql](https://www.postgresql.org) database.

### 4. Connecting main website, CMS and database
Everything is connected by the [Nginx](https://nginx.org) proxy server.

### 5. SSL
The certificate for Secure Sockets Layer (SSL) connection (i.e. the `https://` connection is provided by the [Let's Encrypt](https://letsencrypt.org), a nonprofit Certificate Authority. They have implemented the `certbot` which provides (semi-)automated way for us to apply for a certificate.

!!! warning

    The certbot implementation is buggy, and we are looking for permanent solution. For now, you will have to manually update the certificate.

### 6. Media Management
The images of the website are served by [Cloudinary](https://cloudinary.com), an external media management service. This is to optimise the speed of building the website.

### Docker
With the exception of media management, everything listed above could be built using [the Docker engine](https://www.docker.com). Therefore, the only thing you have to install for development is the Docker engine. Once this is installed, you can run suitable commands to install the remaining website parts for local development/production.

!!! warning

    We will [upgrade the content management system](https://strapi.io/five) during the Christmas vacation to version 5. We may also consider using [Typescript](https://www.typescriptlang.org) over Javascript. As a result the documentation may need to be updated.

