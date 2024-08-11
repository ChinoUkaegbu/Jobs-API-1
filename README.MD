<a id="readme-top"></a>


<!-- PROJECT SHIELDS -->
[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]



<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/ChinoUkaegbu/Jobs-API-1">
    <img src="/assets_readme/logo-job-seeker.png" alt="Logo" width="80" height="80">
  </a>

<h3 align="center">Jobs API</h3>

  <p align="center">
    A RESTful API for managing job applications
    <br />
    <a href="https://github.com/ChinoUkaegbu/Jobs-API-1"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://jobs-api-1-9fp1.onrender.com/api-docs">View Demo</a>
    ·
    <a href="https://github.com/ChinoUkaegbu/Jobs-API-1/issues/new?labels=bug&template=bug-report---.md">Report Bug</a>
    ·
    <a href="https://github.com/ChinoUkaegbu/Jobs-API-1/issues/new?labels=enhancement&template=feature-request---.md">Request Feature</a>
  </p>
</div>



<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li><a href="#getting-started">Getting Started</a></li>
      <ul>
        <li><a href="#installation">Installation</a></li>
      </ul>
    <li><a href="#features">Features</a></li>
    <li><a href="#usage">Usage</a></li>
      <ul>
        <li><a href="#auth-endpoints">Auth Endpoints</a></li>
        <li><a href="#job-endpoints-requires-jwt">Job Endpoints (Requires JWT)</a></li>
      </ul>
    <li><a href="#how-it-works">How it Works</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

[![Jobs API Screen Shot][product-screenshot]](https://jobs-api-1-9fp1.onrender.com)

✨ This is a RESTful API for managing job listings, built using Node.js, Express, and MongoDB. he API provides endpoints for user authentication (register and login) and job management (CRUD operations). It uses JSON Web Tokens (JWT) for secure access to protected endpoints. The project is hosted on Render, and the Swagger UI documentation is available online for testing the endpoints.✨ 

<p align="right">(<a href="#readme-top">back to top</a>)</p>



### Built With

* [![Node][Node.js]][Node-url]
* [![Express][Express.js]][Express-url]
* [![MongoDB][MongoDB.com]][MongoDB-url]
* [![Swagger][Swagger.com]][Swagger-url]
* [![Render][Render.com]][Render-url]


<p align="right">(<a href="#readme-top">back to top</a>)</p>


<!-- GETTING STARTED -->
## Getting Started

You can interact with the API endpoints <a href="https://jobs-api-1-9fp1.onrender.com/api-docs/">here</a>. Please note that the app is being hosted on Render and may take around a minute or more to spin up. To run locally, skip to <a href="#installation">installation</a>.

### Installation

1. Clone the repo
   ```sh
   git clone https://github.com/ChinoUkaegbu/Jobs-API-1.git
   ```
2. Install NPM packages
   ```sh
   npm install
   ```
3. Set up environment variables:

   Create a .env file in the root of the project with the following variables:
   ```ini
   MONGO_URI=your_mongodb_uri
   JWT_SECRET=your_jwt_secret
   JWT_LIFETIME=your_jwt_lifetime
   ```
   The JWT_LIFETIME is how long the token will be valid for and can be set to values such as '30d' (30 days). Refer to json-web-token <a href="https://www.npmjs.com/package/jsonwebtoken#:~:text=expiresIn%3A%20expressed%20in%20seconds%20or%20a%20string%20describing%20a%20time%20span%20vercel/ms">documentation</a> for more info.

4. Run the project
   ```sh
   npm start
   ```

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- FEATURES -->
## Features

### User Authentication:
- Register a new user with a name, email, and password (hashed using bcrypt).
- Login with email and password to receive a JSON Web Token (JWT) for authenticated access.

### Job Management:
- Create, read, update, and delete job listings.
- All job-related endpoints require a valid JWT for access.

<p align="right">(<a href="#readme-top">back to top</a>)</p>


<!-- USAGE EXAMPLES -->
## Usage
Once the server is running, you can use the following endpoints:

### Auth Endpoints

- `POST /api/v1/auth/register`: Register a new user and receive a JSON Web Token (JWT).
- `POST /api/v1/auth/login`: Login and receive a JWT.

### Job Endpoints (Requires JWT)

- `GET /api/v1/jobs`: Get all jobs for the authenticated user.
- `GET /api/v1/jobs/:id`: Get a single job by ID.
- `POST /api/v1/jobs`: Create a new job.
- `PATCH /api/v1/jobs/:id`: Update an existing job by ID.
- `DELETE /api/v1/jobs/:id`: Delete a job by ID.


<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- TECHNICAL-ISH EXPLANATION -->
## How it Works


<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- ROADMAP -->
## Roadmap

- [ ] Format 'home' page
- [ ] Add more properties to jobs

See the [open issues](https://github.com/ChinoUkaegbu/Jobs-API-1/issues) for a full list of proposed features (and known issues).

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE.txt` for more information.

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- CONTACT -->
## Contact

Chino Ukaegbu - [@twitter_handle](https://twitter.com/twitter_handle) - chinoukaegbu@gmail.com

Project Link: [https://github.com/ChinoUkaegbu/Jobs-API-1](https://github.com/ChinoUkaegbu/Jobs-API-1)

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

- People who ask questions on Stack Overflow...and people who respond - where would the debugging community be without you 🥹?

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/ChinoUkaegbu/Jobs-API-1.svg?style=for-the-badge
[contributors-url]: https://github.com/ChinoUkaegbu/Jobs-API-1/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/ChinoUkaegbu/Jobs-API-1.svg?style=for-the-badge
[forks-url]: https://github.com/ChinoUkaegbu/Jobs-API-1/network/members
[stars-shield]: https://img.shields.io/github/stars/ChinoUkaegbu/Jobs-API-1.svg?style=for-the-badge
[stars-url]: https://github.com/ChinoUkaegbu/Jobs-API-1/stargazers
[issues-shield]: https://img.shields.io/github/issues/ChinoUkaegbu/Jobs-API-1.svg?style=for-the-badge
[issues-url]: https://github.com/ChinoUkaegbu/Jobs-API-1/issues
[license-shield]: https://img.shields.io/github/license/ChinoUkaegbu/Jobs-API-1.svg?style=for-the-badge
[license-url]: https://github.com/ChinoUkaegbu/Jobs-API-1/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://www.linkedin.com/in/chinonyerem-ukaegbu
[product-screenshot]: assets_readme/Jobs_API_Documentation.png
[Node.js]: https://img.shields.io/badge/Node%20js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white
[Node-url]: https://nodejs.org/en
[Express.js]: https://img.shields.io/badge/Express%20js-000000?style=for-the-badge&logo=express&logoColor=white
[Express-url]: https://expressjs.com/
[MongoDB.com]: https://img.shields.io/badge/MongoDB-%234ea94b.svg?style=for-the-badge&logo=mongodb&logoColor=white
[MongoDB-url]: https://www.mongodb.com/
[Swagger.com]: https://img.shields.io/badge/-Swagger-%23Clojure?style=for-the-badge&logo=swagger&logoColor=white
[Swagger-url]: https://swagger.io/
[Render.com]: https://img.shields.io/badge/Render-%46E3B7.svg?style=for-the-badge&logo=render&logoColor=white
[Render-url]: https://render.com/
