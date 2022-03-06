
<div id="top"></div>
<!--
*** Thanks for checking out my project
*** Don't forget to give the project a star!
*** Thanks again! Now go create something AMAZING! :D
-->



<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->
[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]



<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/saidalbouti99/brownie-simple-storage">
    <img src="https://www.google.com/search?q=solidity+symbol&sxsrf=APq-WBsaizo6dEXhWG-Uo5Z9OAhYROD4-g:1646578259757&source=lnms&tbm=isch&sa=X&ved=2ahUKEwiJ3ZGC3rH2AhUg63MBHcWwDLsQ_AUoAXoECAEQAw&biw=1536&bih=662&dpr=1.25#imgrc=Ahvg8X_JVTzJHM" alt="Logo" width="80" height="80">
  </a>

<h3 align="center">Brownie Simple Storage</h3>

  <p align="center">
    A simple storage smart contract deployed using Brownie
    <br />
    <a href="https://github.com/saidalbouti99/brownie-simple-storage"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://github.com/saidalbouti99/brownie-simple-storage">View Demo</a>
    ·
    <a href="https://github.com/saidalbouti99/brownie-simple-storage/issues">Report Bug</a>
    ·
    <a href="https://github.com/saidalbouti99/brownie-simple-storage/issues">Request Feature</a>
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

 A simple storage smart contract to store and retrieve number in the Ethereum blockchain using Solidity and Python and deployed using Brownie

<p align="right">(<a href="#top">back to top</a>)</p>



### Built With

* [Solidity](https://soliditylang.org/)
* [Python](https://www.python.org/)
* [Brownie](https://eth-brownie.readthedocs.io/en/stable/)

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- GETTING STARTED -->
## Getting Started

This is an example of how you may give instructions on setting up your project locally.
To get a local copy up and running follow these simple example steps.


### Installation

1. Install Brownie

```bash
python3 -m pip install --user pipx
python3 -m pipx ensurepath
# restart your terminal
pipx install eth-brownie
```
Or, if that doesn't work, via pip
```bash
pip install eth-brownie
```

2. Clone this
```bash
git clone https://github.com/PatrickAlphaC/brownie_simple_storage
cd brownie_simple_storage
```
3. Add your metamask to the brownie accounts at the `0` index

```bash
brownie accounts new 0
```
You'll be prompted to add your private key:
`0xa5555555555555a09215803a6b540f1e054797eeda2eec6d49076760d48e7589`
And a password, and you can see your new added account with `brownie accounts list`

Or, export your `PRIVATE_KEY` as an environment variable, and uncomment the line:
```python
# account = accounts.add(config["wallets"]["from_key"])
```
and comment the line:
```python
account = accounts[0]
```

4. Testing

```bash
brownie test
```

5. Running scripts

```bash
brownie run scripts/deploy.py
```

6. Deploy to a testnet

Add your `WEB3_INFURA_PROJECT_ID` from [Infura](https://infura.io/) to your `.env` and run 
```bash
source .env
``` 
To set your environment variable. You can check you've done it correctly with:
```bash
echo $WEB3_INFURA_PROJECT_ID
```
Change the `deploy_simple_storage` function in `deploy.py` to look like:
```
account = accounts.add(config["wallets"]["from_key"])
# account = accounts.load("id")
# account = accounts[0]
```

Then run:
```
brownie run scripts/deploy.py --network rinkeby
```

Make sure you have some testnet ETH. You can find faucets in the [Chainlink Documenatation](https://docs.chain.link/docs/link-token-contracts/)



   ```

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- USAGE EXAMPLES -->
## Usage

Use this space to show useful examples of how a project can be used. Additional screenshots, code examples and demos work well in this space. You may also link to more resources.

_For more examples, please refer to the [Documentation](https://example.com)_

<p align="right">(<a href="#top">back to top</a>)</p>



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

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE.txt` for more information.

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- CONTACT -->
## Contact

Project Link: [https://github.com/saidalbouti99/brownie-simple-storage](https://github.com/saidalbouti99/brownie-simple-storage)

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

* [PatrickAlphaC](https://github.com/PatrickAlphaC)


<p align="right">(<a href="#top">back to top</a>)</p>



<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/github_username/repo_name.svg?style=for-the-badge
[contributors-url]: https://github.com/github_username/repo_name/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/github_username/repo_name.svg?style=for-the-badge
[forks-url]: https://github.com/github_username/repo_name/network/members
[stars-shield]: https://img.shields.io/github/stars/github_username/repo_name.svg?style=for-the-badge
[stars-url]: https://github.com/github_username/repo_name/stargazers
[issues-shield]: https://img.shields.io/github/issues/github_username/repo_name.svg?style=for-the-badge
[issues-url]: https://github.com/github_username/repo_name/issues
[license-shield]: https://img.shields.io/github/license/github_username/repo_name.svg?style=for-the-badge
[license-url]: https://github.com/github_username/repo_name/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/linkedin_username
[product-screenshot]: images/screenshot.png
