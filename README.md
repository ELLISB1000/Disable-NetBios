<!-- Back to top link-->
<a name="readme-top"></a>

[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]


<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/ELLISB1000/Disable-NetBios">
    <img src="Public/logo.png" alt="Logo" width="400" height="400">
  </a>

<h3 align="center">Disable-NetBios</h3>

  <p align="center">
    A PowerShell script to detect and disable NetBios on all Interfaces.
    <br />
    <a href="https://github.com/ELLISB1000/Disable-NetBios/issues">Report Bug</a>
    ·
    <a href="https://github.com/ELLISB1000/Disable-NetBios/issues">Request Feature</a>
  </p>
</div>



<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

A script that can be deployed with Intune as a remediation to detect clients with NetBios enabled on any interface. This is done by checking for the registry key for each interface for the value of the key `NetbiosOptions`. If NetBios is detected as enabled the `Disable-NetBios.ps1` script will loop through all the interfaces and set the value to `2` which will disable NetBios after a system restart.

<p align="right">(<a href="#readme-top">back to top</a>)</p>


<!-- GETTING STARTED -->
## Getting Started

To get a local copy up and running follow these simple example steps.


### Prerequisites

None

### Installation

1. Browse to the folder you store your scripts `e.g. cd C:\Script`
2. Clone the repo
   ```powershell
   Invoke-WebRequest -Uri https://raw.githubusercontent.com/ELLISB1000/Disable-NetBios/main/Detect-NetBios.ps1 -OutFile .\Detect-NetBios.ps1
   Invoke-WebRequest -Uri https://raw.githubusercontent.com/ELLISB1000/Disable-NetBios/main/Disable-NetBios.ps1 -OutFile .\Disable-NetBios.ps1
   ```

<p align="right">(<a href="#readme-top">back to top</a>)</p>


<!-- USAGE EXAMPLES -->
## Usage

For information on how to set this up as a remediation script in Intune please see the following guide:

[Remediation](https://ellisbarrett.com/blog/Disable-NetBioss)

<p align="right">(<a href="#readme-top">back to top</a>)</p>


<!-- ROADMAP -->
## Roadmap

- [X] Create detection script so this can be deployed as a remediation

See the [open issues](https://github.com/ELLISB1000/Disable-NetBios/issues) for a full list of proposed features (and known issues).

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

Distributed under the MIT License. See `LICENSE` for more information.

<p align="right">(<a href="#readme-top">back to top</a>)</p>


<!-- CONTACT -->
## Contact

[Ellis Barrett](https://ellisbarrett.com)

<p align="right">(<a href="#readme-top">back to top</a>)</p>


<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/ELLISB1000/Disable-NetBios.svg?style=for-the-badge
[contributors-url]: https://github.com/ELLISB1000/Disable-NetBios/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/ELLISB1000/Disable-NetBios.svg?style=for-the-badge
[forks-url]: https://github.com/ELLISB1000/Disable-NetBios/network/members
[stars-shield]: https://img.shields.io/github/stars/ELLISB1000/Disable-NetBios.svg?style=for-the-badge
[stars-url]: https://github.com/ELLISB1000/Disable-NetBios/stargazers
[issues-shield]: https://img.shields.io/github/issues/ELLISB1000/Disable-NetBios.svg?style=for-the-badge
[issues-url]: https://github.com/ELLISB1000/Disable-NetBios/issues
[license-shield]: https://img.shields.io/github/license/ELLISB1000/Disable-NetBios.svg?style=for-the-badge
[license-url]: https://github.com/ELLISB1000/Disable-NetBios/blob/master/LICENSE
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/ellis-barrett
