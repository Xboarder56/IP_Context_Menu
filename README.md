# IP_Context_Menu
Custom IP Context Menu for QRadar (Right Click Menu)

This repo contains the custom IP context menu I utilize with my QRadar instance running in my homelab. These OSINT sources I utilize daily when performing incident response. If you have any questions you can create an issue for the GitHub project or open a question/reply on the IBM QRadar CE forms located at: https://ibm.biz/qradarceforums

# OSINT Sources:
  - [AbuseIPDB](https://www.abuseipdb.com/)
  - [AlienVault OTX](https://otx.alienvault.com/)
  - [Censys](https://censys.io/)
  - [Cisco Talos](https://talosintelligence.com/)
  - [Google](https://google.com)
  - [GreyNoise](https://greynoise.io/)
  - [HackerTarget](https://HackerTarget.com/)
  - [McAfee](https://www.mcafee.com/enterprise/en-us/threat-center.html)
  - [MxToolbox](https://mxtoolbox.com)
  - [SANS ISC](https://isc.sans.edu/ipinfo.html)
  - [Shodan](https://www.shodan.io/)
  - [Traceroute](https://en.wikipedia.org/wiki/Traceroute)
  - [Threat Crowd](https://www.threatcrowd.org/)
  - [ThreatMiner](https://www.threatminer.org/)
  - [Virus Total](https://www.virustotal.com/)
  - [X-Force Exchange Lookup](https://exchange.xforce.ibmcloud.com/)

# Install Guide
1. Using SSH, log in to the QRadar Console as the root user.
2. cp /opt/qradar/conf/ip_context_menu.xml /opt/qradar/conf/ip_context_menu.xml.bak
3. wget -nv -O /opt/qradar/conf/ip_context_menu.xml https://raw.githubusercontent.com/Xboarder56/IP_Context_Menu/master/ip_context_menu.xml
4. systemctl restart tomcat

# Change Log
  - 05-22-2019 - Fixed mapping greynoise and google to the wrong lookup links
  - 04-18-2019 - Added MxToolbox ARIN Lookup and HackerTarget ReverseIP Lookup
  - 04-14-2019 - Initial creation of custom IP Context Menu

# Sources/References
- https://www.ibm.com/support/knowledgecenter/en/SS42VS_7.3.2/com.ibm.qradar.doc/t_CUSTOMIZING_THE_RIGHT_CLICK_MENU.html
