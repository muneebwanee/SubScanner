# SubScanner
An automation tool that scans sub-domains, sub-domain takeover and then filters out xss, ssti, ssrf and more injection point parameters.<br/>

+ **Requirements:** Go Language, Python 2.7 or Python 3.
+ **System requirements:** Recommended to run on vps with 1VCPU and 2GB ram.
+ **Tools used - You must need to install these tools to use this script**<br/>

  + [SubFinder](https://github.com/projectdiscovery/subfinder)
  + [Sublist3r](https://github.com/aboul3la/Sublist3r)
  + [GF Patterns](https://github.com/1ndianl33t/Gf-Patterns)
  + [Get Title](https://github.com/tomnomnom/hacks/tree/master/get-title)
  + [Gau](https://github.com/lc/gau)
  + [Subzy](https://github.com/LukaSikic/subzy)
  + [Subjack](https://github.com/haccer/subjack): save [fingerprints.json](https://github.com/haccer/subjack/blob/master/fingerprints.json) file into ~/tools/ directory.
  + [Assetfinder](https://github.com/tomnomnom/assetfinder)
  + [HTTPX](https://github.com/projectdiscovery/httpx)
  + [Waybackurls](https://github.com/tomnomnom/waybackurls)
  
+ **Installation**
```sh
git clone https://github.com/muneebwanee/SubScanner.git && cd SubScanner/ && chmod +x SubScanner && mv SubScanner /usr/local/bin/
```

+ **Usage**
```sh
SubScanner -d target.com -f filename
```

### About SubScanner
I made this tool to automate my recon and save my time. It really give me headache always type such command and then wait to complete one command and I type other command. So I collected some of the tools which is widely used in the bugbounty field. In this script I used Assetfinder, get-titles, httprobe, subjack, subzy, sublister, gau and gf patterns.<br/> 
The script first enumerates all the subdomains of the give target domain using assetfinder and sublister then filters all live domains from the whole subdomain list then it extarct titles of the subdomains using get-title then it scans for subdomain takeover using subjack and subzy. Then it uses gau to extract paramters of the given subdomains then it use gf patterns to filters xss, ssti, ssrf, sqli params from that given subdomains. Then it'll save all the output in a text file like target-xss.txt. <bR/>

![forthebadge](https://forthebadge.com/images/badges/open-source.svg) 
![forthebadge](https://forthebadge.com/images/badges/built-with-love.svg)

#### Thanks to the authors of the tools used in this script.
[@muneebwanee](https://github.com/muneebwanee) [@thedeepnet](https://github.com/thedeepnet)



**Warning:** This code was originally created for personal use, it generates a substantial amount of traffic, please use with caution.

<p align="center">
<a href="#"><img title="Version" src="https://img.shields.io/badge/Version-1.0-green.svg?style=flat-square"></a>
<a href="https://github.com/muneebwanee"><img title="Followers" src="https://img.shields.io/github/followers/muneebwanee?color=blue&style=flat-square"></a>
<a href="https://twitter.com/muneebwanee"><img title="Twitter" src="https://img.shields.io/twitter/follow/muneebwanee?style=social"></a>
<a href="https://twitter.com/the_deepnet"><img title="Contributer" src="https://img.shields.io/twitter/follow/the_deepnet?label=%40the_deepnet&style=social"></a>
<a href="https://instagram.com/muneebwanee"><img title="Instagram" src="https://img.shields.io/badge/IG-%40muneebwanee-red?style=for-the-badge&logo=instagram"></a>
<a href="https://linkedin.com/in/muneebwanee"><img title="LinkedIn" src="https://img.shields.io/badge/LinkedIn%20-muneebwanee-orange?colorA=%23ff9696&colorB=%237E7B4E&style=for-the-badge"></a>
<a href="https://m.me/me.muneebwanee"><img title="Facebook" src="https://img.shields.io/badge/Chat-Messenger-blue?style=for-the-badge&logo=messenger"></a>
<a href="https://github.com/muneebwanee"><img title="GitHub" src="https://img.shields.io/badge/Github-Muneeb--Wanee-green?style=for-the-badge&logo=github"></a>
<a href="https://www.buymeacoffee.com/muneebwanee" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: 41px !important;width: 174px !important;box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;-webkit-box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;" ></a>
</p>

