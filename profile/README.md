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

API's:

* [![Python]][Python-url]
* [![FastAPI]][FastAPI-url]
* [![MongoDB]][MongoDB-url]

Web application:

* [![Yarn]][Yarn-url]
* [![Vite]][Vite-url]
* [![Vue.js]][Vue.js-url]
* [![Typescript]][Typescript-url]
* [![Tailwind]][Tailwind-url]

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

<img src="https://github.com/f1betting/.github/raw/main/docs/architecture_basic.jpg">

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

[Python]: https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54

[Python-url]: https://python.org

[FastAPI]: https://img.shields.io/badge/FastAPI-005571?style=for-the-badge&logo=fastapi

[FastAPI-url]: https://fastapi.tiangolo.com/

[MongoDB]: https://img.shields.io/badge/MongoDB-%234ea94b.svg?style=for-the-badge&logo=mongodb&logoColo

r=white

[MongoDB-url]: https://www.mongodb.com/

[Yarn]: https://img.shields.io/badge/yarn-%232C8EBB.svg?style=for-the-badge&logo=yarn&logoColor=white

[Yarn-url]: https://yarnpkg.com/

[Vite]: https://img.shields.io/badge/vite-%23646CFF.svg?style=for-the-badge&logo=vite&logoColor=white

[Vite-url]: https://vitejs.dev/

[Vue.js]: https://img.shields.io/badge/vuejs-%2335495e.svg?style=for-the-badge&logo=vuedotjs&logoColor=%234FC08D

[Vue.js-url]: https://vuejs.org/

[Typescript]: https://img.shields.io/badge/typescript-%23007ACC.svg?style=for-the-badge&logo=typescript&logoColor=white

[Typescript-url]: https://www.typescriptlang.org/

[Tailwind]: https://img.shields.io/badge/tailwindcss-%2338B2AC.svg?style=for-the-badge&logo=tailwind-css&logoColor=white

[Tailwind-url]: https://tailwindcss.com/
