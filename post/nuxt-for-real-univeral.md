# Nuxt-related : are we really reach the universal SSR? Template-module-builder for other backend
---


<!-- omit in toc -->
- [# Nuxt-related : are we really reach the universal SSR? Template-module-builder for other backend](#h1-idnuxt-related--are-we-really-reach-the-universal-ssr-template-module-builder-for-other-backend-342nuxt-related--are-we-really-reach-the-universal-ssr-template-module-builder-for-other-backendh1)
- [- Remark / reference.](#ulliremark--referenceliul)
- [Introduction](#introduction)
- [Reason for not using front-end JS framework](#reason-for-not-using-front-end-js-framework)
  - [Single Page Application (SPA) cause poor SEO](#single-page-application-spa-cause-poor-seo)
  - [Nodejs is taking large memory as application](#nodejs-is-taking-large-memory-as-application)
- [So, Advanced SSR framework is built, but why not?](#so-advanced-ssr-framework-is-built-but-why-not)
  - [Remark / reference.](#remark--reference)
---
## Introduction

Over and over years, from jquery Angular v1 to Vue v1, from Vue v2 to Nuxt, our client side webpage client have been grown powerful, powerful that improving the UX preformance, e.g. smooth loading large Content Resource, great animation with DOM element, SVG and Canvas.

However, it is no doubt that the Nodejs / Python is not major for backend servver in market,(even me, I am not so honic in Nodejs as server-side, use Golang instead ;) ). Java (Spring/Spring Boot), CSharp (ASP dot net MVC5) and PHP (laraval5 / codeIgnore) are still running smooth and stable for those enterprises and vendor companies. In server-side, yes it is unbeatable, but it also cause the performance in client-side degrading. 

It make me annoyed but it is no way to against this destiny. No one, or no team is willing speading much and much time in mutliple skill in same project, even a large scale company, it took 2~3 team for multiple language in similar case.

<!-- OK, so why not take a look to the reason that not using front-end JS framework to enhance performance? -->

## Reason for not using front-end JS framework

### Single Page Application (SPA) cause poor SEO

Since many of front-end JS framework using Virual DOM, or generate conent in client-side browser runtime, content is not optimize for search engine.

### Nodejs is taking large memory as application

Nodejs Application have large file size in library, while the other server may build as binary. 

https://www.techempower.com/benchmarks/#section=data-r19&hw=ph&test=fortune&l=zik0ov-1r

## So, Advanced SSR framework is built, but why not?

As the SPA app is having SEO issue and server, SSR framework is built from those framework, [Gasby.js](),  [Nextjs]() and [Nuxtjs]() are building on top of this issues and overcome. 
so, what next issue is, **"how to speed up in multiple language framework"**



as the fans of Nuxt.js, I have an idea: well, **why not build a module for generating SSR template**
;

yup, it may sound silly for those backend guys, but, just give a try, it should be better than Vue.js v1, right?

# Plan 
everything have plan, so it should run the project under expected...

here is the plan :
- build as directive/Component for front-end development and production mode
- write the generic wrapper for converting the conted
- pick a backend server framework as a start and testing
  - php : native (basic) / laravel
  - golang : Gin (basic) / Gorilla / Goji / Iris
  - java : Jsp (basic) / Rocker / Freemarker
  - csharp : (Standard Razor, Blazor) 


### Remark / reference. 

https://www.robertcooper.me/comparing-nextjs-and-gatsbyjs-static-site-generation


https://web.dev/prerender-with-react-snap/