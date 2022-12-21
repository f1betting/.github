<a name="readme-top"></a>

<div>
<h3 align="center">F1Betting</h3>

  <p align="center">
    Betting on Formula 1 races!
    <br />
    <a href="https://github.com/orgs/f1betting/repositories">View repositories</a>
  </p>
</div>



<!-- TABLE OF CONTENTS -->

## 📋 Table of contents

- [ℹ️ About The Project](#-about-the-project)
    - [🚧 Built With](#built-with)
- [🚦 Repository statuses](#-repository-statuses)
    - [🐙 OpenAPItoKrakenD](#-openapitokrakend)
    - [🏆 F1Betting](#-f1betting)
    - [🚗 F1API](#-f1api)
    - [💻 F1FrontEnd](#-f1frontend)
- [🚀 Usage ](#-usage)
- [🏛️ Architecture ](#-architecture)
    - [🚜 Basic architecture](#-basic-architecture)
    - [🏎️ Advanced architecture](#-advanced-architecture)
    - [📊 Sequence diagram](#-sequence-diagram)
- [📜 License](#-license)

<!-- ABOUT THE PROJECT -->

## ℹ️ About The Project

This project contains the repositories for the research part of my internship about API and API gateways.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

### 🚧 Built With

APIs:

* [![Python]][Python-url]
* [![FastAPI]][FastAPI-url]
* [![MongoDB]][MongoDB-url]

Web application:

* [![Yarn]][Yarn-url]
* [![Vite]][Vite-url]
* [![Vue.js]][Vue.js-url]
* [![Typescript]][Typescript-url]
* [![Tailwind]][Tailwind-url]

Automation and deployment:

* [![GitHub-Actions]][GitHub-Actions-url]
* [![Google-Cloud]][Google-Cloud-url]
* [![Krakend]][Krakend-url]

<p align="right">(<a href="#readme-top">back to top</a>)</p>


<!-- REPOSITORY STATUS -->

## 🚦 Repository statuses

### 🐙 OpenAPItoKrakenD

A tool to batch-convert OpenAPI 3.0 files to a flexible KrakenD configuration

<img alt="SonarCloud coverage" src="https://sonarcloud.io/api/project_badges/measure?project=f1betting_OpenAPItoKrakenD&metric=coverage">
<img alt="SonarCloud quality gate" src="https://sonarcloud.io/api/project_badges/measure?project=f1betting_OpenAPItoKrakenD&metric=alert_status">
<img alt="SonarCloud code smells" src="https://sonarcloud.io/api/project_badges/measure?project=f1betting_OpenAPItoKrakenD&metric=code_smells">
<img alt="GitHub Workflow Status" src="https://img.shields.io/github/actions/workflow/status/f1betting/OpenAPItoKrakenD/python_on_push_master.yml?label=Build&branch=main">

### 🏆 F1Betting

An API to do bets with your friends about F1 race results!

<img alt="GitHub tag (latest by date)" src="https://img.shields.io/github/v/tag/f1betting/f1betting?label=Version">
<img alt="Docker version" src="https://img.shields.io/docker/v/nieko3/f1betting/latest?label=Docker%20version">
<br>
<img alt="SonarCloud coverage" src="https://sonarcloud.io/api/project_badges/measure?project=f1betting_F1Betting&metric=coverage">
<img alt="SonarCloud quality gate" src="https://sonarcloud.io/api/project_badges/measure?project=f1betting_F1Betting&metric=alert_status">
<img alt="SonarCloud code smells" src="https://sonarcloud.io/api/project_badges/measure?project=f1betting_F1Betting&metric=code_smells">
<img alt="GitHub Workflow Status" src="https://img.shields.io/github/actions/workflow/status/f1betting/F1Betting/python_on_push_master.yml?label=Build&branch=main">

### 🚗 F1API

A more user-friendly way to use ergast.com

<img alt="GitHub tag (latest by date)" src="https://img.shields.io/github/v/tag/f1betting/f1api?label=Version">
<img alt="Docker version" src="https://img.shields.io/docker/v/nieko3/f1api/latest?label=Docker%20version">
<br />
<img alt="SonarCloud coverage" src="https://sonarcloud.io/api/project_badges/measure?project=f1betting_F1API&metric=coverage">
<img alt="SonarCloud quality gate" src="https://sonarcloud.io/api/project_badges/measure?project=f1betting_F1API&metric=alert_status">
<img alt="SonarCloud code smells" src="https://sonarcloud.io/api/project_badges/measure?project=f1betting_F1API&metric=code_smells">
<img alt="GitHub Workflow Status" src="https://img.shields.io/github/actions/workflow/status/f1betting/F1API/python_on_push_master.yml?label=Build&branch=main">

### 💻 F1FrontEnd

A basic front-end to interact with the F1Betting API

<img alt="SonarCloud coverage" src="https://sonarcloud.io/api/project_badges/measure?project=f1betting_F1FrontEnd&metric=coverage">
<img alt="SonarCloud quality gate" src="https://sonarcloud.io/api/project_badges/measure?project=f1betting_F1FrontEnd&metric=alert_status">
<img alt="SonarCloud code smells" src="https://sonarcloud.io/api/project_badges/measure?project=f1betting_F1FrontEnd&metric=code_smells">

<p align="right">(<a href="#readme-top">back to top</a>)</p>


<!-- USAGE EXAMPLES -->

## 🚀 Usage

To view more information about each project, please check out every individual repositories' ``README.md`` to learn more
about each project.

<p align="right">(<a href="#readme-top">back to top</a>)</p>


<!-- ARCHITECTURE EXAMPLES -->

## 🏛️ Architecture

The recommended way to deploy the full application is by using an API gateway. This allows for detailed logging &
metrics, as well as extra security.

The APIs and KrakenD gateway are currently automatically deployed to Google Cloud Run via GitHub Actions. To view more
information about the KrakenD deployment, check out [OpenAPItoKrakenD](https://github.com/f1betting/OpenAPItoKrakenD)

### 🚜 Basic architecture

The basic architecture does not utilize an API gateway. Instead, all the API's call eachother directly. This is the
easiest way to get started.

The MongoDB database can be run using Docker or you can use a cloud environment such as MongoDB Atlas.

<img src="https://github.com/f1betting/.github/raw/main/docs/architecture_basic.jpg">

### 🏎️ Advanced architecture

Alternatively you could use an API gateway such as [KrakenD](https://www.krakend.io/)
or [Gravitee](https://www.gravitee.io/). This allows for detailed logging &
metrics, as well as extra security.

The MongoDB database can be run using Docker or you can use a cloud environment such as MongoDB Atlas.

<img src="https://github.com/f1betting/.github/raw/main/docs/architecture_gateway.jpg">

_Note that the F1Betting and F1API APIs communicate to each other through the gateway._

### 📊 Sequence diagram

Below is a sequence diagram that utilizes the gateway architecture. The processes shown here are the sign-in process
(flow 1) and the process of creating a new bet (flow 2).

<img src="https://github.com/f1betting/.github/raw/main/docs/sequence_diagram.png">

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- LICENSE -->

## 📜 License

Distributed under the MIT License. See `LICENSE.md` under each repository for more information.

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->

[Python]: https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=white

[Python-url]: https://python.org

[FastAPI]: https://img.shields.io/badge/FastAPI-005571?style=for-the-badge&logo=fastapi&logoColor=white

[FastAPI-url]: https://fastapi.tiangolo.com/

[MongoDB]: https://img.shields.io/badge/MongoDB-%234ea94b.svg?style=for-the-badge&logo=mongodb&logoColor=white

[MongoDB-url]: https://www.mongodb.com/

[Yarn]: https://img.shields.io/badge/yarn-%232C8EBB.svg?style=for-the-badge&logo=yarn&logoColor=white

[Yarn-url]: https://yarnpkg.com/

[Vite]: https://img.shields.io/badge/vite-%23646CFF.svg?style=for-the-badge&logo=vite&logoColor=white

[Vite-url]: https://vitejs.dev/

[Vue.js]: https://img.shields.io/badge/vuejs-%2335495e.svg?style=for-the-badge&logo=vuedotjs&logoColor=white

[Vue.js-url]: https://vuejs.org/

[Typescript]: https://img.shields.io/badge/typescript-%23007ACC.svg?style=for-the-badge&logo=typescript&logoColor=white

[Typescript-url]: https://www.typescriptlang.org/

[Tailwind]: https://img.shields.io/badge/tailwindcss-%2338B2AC.svg?style=for-the-badge&logo=tailwind-css&logoColor=white

[Tailwind-url]: https://tailwindcss.com/

[GitHub-Actions]: https://img.shields.io/badge/github%20actions-%232671E5.svg?style=for-the-badge&logo=githubactions&logoColor=white

[GitHub-Actions-url]: https://github.com/features/actions

[Google-Cloud]: https://img.shields.io/badge/Google%20Cloud%20Run-%234285F4.svg?style=for-the-badge&logo=google-cloud&logoColor=white

[Google-Cloud-url]: https://cloud.google.com/

[KrakenD]: https://img.shields.io/badge/KrakenD-%230c66f2.svg?style=for-the-badge&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgCAMAAABEpIrGAAAABGdBTUEAALGPC/xhBQAAAAFzUkdCAK7OHOkAAAITUExURQAAAP///////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////wl/jeAAAACwdFJOUwDWA+vL5/3v9t364cqp888M2kAggt41qwT0+xyiKbbbmBEZ0yPtnwGGB6qd5eBYtcjGkKjf2eTqxLPNvckQIlIJ0sIUFpH+k0qBH7EX0LATpjRchfKlzPwyQbJ3lq4NJ6QshEn4nI4a2HzmPNdwRFd1Br8Y6WX1Q4unw+LRla9dZm7jYFDcai+4gy3HOJJMo3a5Cmm+wDCHgHOtcWHojHk9tB05mW+XY8FFVs43Jn+g1FohogAAAnpJREFUOMuVU1V74zAQ3KDjJE0abrjMzMzMzMx4zMzMzMw4P/EkO8213/Xl9KDZ1YxX45VE9D9j7lOtmCF++dC8IxsTAUBYV6wLDFPb/+GjgayqJDnuuulG2na63gBXCg/efRx4O9F0oeeIpyB2C18JvZWjswYwCcIQUOwThPgwn6ItjOKYDOHFJA/qzqiZEZVyU+CABA1IpIr8zd1PAeoQn4ZIDlZEU7XWuIhZovNlJ+k0kCvxFejr6VfYSNAQPYKTPDnkg0GnpREghguuzF/DxMV0Lw6yxIiXmPJikSghg8YQwQW42qIlJVwmyajdF0sb3NNtNnXwoAqTl1Eiqsd1RC05wQfjbygK0xSlVxDNYDdRHlNd6lco77jtwAF1hw5F/m9ww+Tl1fOIzCr5XzKBEqk1cw5Y/SW/pUUN+1NDHNHK6vJXSS2PACqJlmrEKjphIUofpFQEyvHDpQu3VqGnGW3QiLW2QlahNgVjRLUmgiWswLCPWQvWjBYQlRd4ecUVkBOaGxJte4hfdiZIMJYWEy2AhOWKnzATVWtgSbRHx0FV+l25Ct3QlDuR6D388R4gSLSxRq/z2SmmN1AfKNJ1t3UJh/l+2XTv6WeiQnanWCodXJZs+Jh0zNOo51A8bxtBcsikalD2Kp1FEhxSUkakLZN5JzI5dGKvlO5BOZtzsRDALVmg1/C5OVxwH/LZF688pvtS2loEGwMl4sJ9yQDMs6HYP4BDw9xswt/OUpcGjSroHGazqAe6+dIuNG699zHX8ez544BCLB09KxmPgKVu+9PJRdGT6lBsTQWa/nl77Z2siQZjjvo4w7b9O77f3u5s8ZyYfbR3y9of/7yzgTeSI9wAAAAASUVORK5CYII=&logoColor=white

[KrakenD-url]: https://www.krakend.io/