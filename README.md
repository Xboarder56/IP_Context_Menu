# IP_Context_Menu
Custom IP Context Menu for QRadar (Right Click Menu)

This repo contains the custom IP context menu I utilize with my QRadar instance running in my homelab. These OSINT sources I utilize daily when performing incident response. If you have any questions you can create an issue for the GitHub project or open a question/reply on the IBM QRadar CE forms located at: https://ibm.biz/qradarceforums

# Install Guide
1. Using SSH, log in to the QRadar Console as the root user.
2. cp /opt/qradar/conf/ip_context_menu.xml /opt/qradar/conf/ip_context_menu.xml.bak
3. wget -nv -O /opt/qradar/conf/ip_context_menu.xml %RAW GITHUB LINK HERE%
4. systemctl restart tomcat

# Change Log
  - 04-14-2019 - Initial creation of custom IP Context Menu

# Sources/References
- https://www.ibm.com/support/knowledgecenter/en/SS42VS_7.3.2/com.ibm.qradar.doc/t_CUSTOMIZING_THE_RIGHT_CLICK_MENU.html
