---
layout: post
title: "How to migrate project from Monolith to Micro-service"
excerpt: "Step by Step info to help in migration"
categories: blog
tags: [ blog ]

date: 2022-05-27T08:08:50-04:00

---

* Follow how Revive was migrated from monolith to micro-service

Current Version

* Setting up [Shop](https://slabstech.github.io/shop/) , using [revive](https://github.com/sachinsshetty/revive) project


June 7 - Version
* samruddhi-react :
  * Migrating Samruddhi project from Single Markdown Page to ReactJS 
  * ReactJS standalone project is deployed to gh-pages.
  * Created a PreProcessor in Java to convert BookData to Json.data_import directory [Source](https://github.com/slabstech/samrudhi-react)
  * Json Data to be loaded into website using Fetch
* shop :
  * Made config changes to refactor project from Revive to Shop
  * Removed spring_boot configs and source code directory.

June 6 - Version
* revive:
  * Create composite github actions to handle Docker multi-stage build issue with Server(SpringBoot+Dropwizard)
  * Now gradle build is run inside the docker container. Server code is copied to docker container.
  * Build task now runs independently and can run in parallel if build task is successful.

June 5 - Version
* revive:
  * Docker push failing as build directory not found in container. Build files are copied from host machine to container.
  * Local push to docker successful, Github actions does not have access to build files from pre-cursor task, Try to build project inside gradle container.
  
June 4 - Version
* revive:
  * Add starter code for Dropwizard. Second option for Server. Dropwizard is suitable for micro-services
  