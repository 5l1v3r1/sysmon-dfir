# Sysmon - DFIR

A curated list of resources for learning about deploying, managing and hunting with Microsoft Sysmon. Contains presentations, deployment methods, configuration file examples, blogs and additional github repositories.


# Sysmon Learning Resources


  * [General](#general)
    * [Presentations](#Presentations)
      * [How to Go from Responding to Hunting with Sysinternals Sysmon - Mark Russinovich](https://onedrive.live.com/view.aspx?resid=D026B4699190F1E6!2843&ithint=file%2cpptx&app=PowerPoint&authkey=!AMvCRTKB_V1J5ow)
      * [Tracking Hackers on Your Network with Sysinternals Sysmon - Mark Russinovich](https://www.rsaconference.com/writable/presentations/file_upload/hta-w05-tracking_hackers_on_your_network_with_sysinternals_sysmon.pdf)
      * [Advanced Incident Detection and Threat Hunting using Sysmon and Splunk Video - Tom Ueltschi](https://youtu.be/vv_VXntQTpE)
      * [Advanced Incident Detection and Threat Hunting using Sysmon and Splunk Slides - Tom Ueltschi](http://security-research.dyndns.org/pub/slides/BotConf/2016/Botconf-2016_Tom-Ueltschi_Sysmon.pdf)
      * [Splunking	the	Endpoint - James Brodsky](https://conf.splunk.com/session/2015/conf2015_Jbrodsky_Splunk_SecurityComplinace_SplunkingTheEndpoint_FINAL.pdf)
      * [Splunking the Endpoint: “Hands on!” Ransomware	Edition - James Brodsky & Dimitri McKay](https://conf.splunk.com/files/2016/slides/splunking-the-endpoint-hands-on.pdf)
    * [Graylog](#graylog)
      * [Ion-Storm Graylog App](https://github.com/ion-storm/sysmon-config)
      * [Back to Basics- Enhance Windows Security with Sysmon and Graylog - Jan Dobersten](https://www.graylog.org/blog/83-back-to-basics-enhance-windows-security-with-sysmon-and-graylog)
    * [ELK](#ELK)
      * [Building a Sysmon Dashboard with an ELK Stack - Roberto Rodriguez](https://cyberwardog.blogspot.com/2017/03/building-sysmon-dashboard-with-elk-stack.html?m=1)
    * [Splunk](#splunk)
      * [Splunk App to assist Sysmon Threat Hunting - Mike Haag](https://github.com/MHaggis/app_splunk_sysmon_hunter)
      * [Splunking the Endpoint - Files from presentation - James Brodsky & Dimitri McKay](https://splunk.app.box.com/v/splunking-the-endpoint)
    * [Deploy Sysmon](#deploy_sysmon)
      * [Sysmon.bat - Ion-Storm](https://github.com/ion-storm/sysmon-config/blob/master/Install%20Sysmon.bat)
      * [Deploying Sysmon through Group Policy - Pablo Delgado](http://syspanda.com/index.php/2017/02/28/deploying-sysmon-through-gpo/)
    * [Sysmon Configuration Files](#sysmon-configuration)
      * [SwiftOnSecurity Sysmon Configuration](https://github.com/SwiftOnSecurity/sysmon-config)
      * [Ion-Storm Graylog App and Sysmon Configuration](https://github.com/ion-storm/sysmon-config/blob/master/sysmonconfig-export.xml)
      * [909Research Blog](http://909research.com/sysmon-the-best-free-windows-monitoring-tool-you-arent-using/)
      * [Decent Security Config](https://decentsecurity.com/enterprise/#/sysmon-enterprise-configuration/)
      * [MalwareArchaeology](https://www.malwarearchaeology.com/logging/)
    * [Blogs](#Blogs)
      * [Explaining and adapting Tay’s Sysmon configuration - Lennart Koopmann](https://medium.com/@lennartkoopmann/explaining-and-adapting-tays-sysmon-configuration-27d9719a89a8#.9u01gmxgh)
      * [Detecting Lateral Movement Using Sysmon and Splunk - David French](http://www.incidentresponderblog.com/2016/09/detecting-lateral-movement-using-sysmon.html)
      * [Setting up Elasticsearch 5.x – Sending Windows Logs using WinLogbeat 5.x Part 2/3 - Pablo Delgado](http://syspanda.com/index.php/2017/02/07/setting-up-elasticsearch-5-x-sending-windows-logs-using-winlogbeat-5-x/)
      * [Advanced Sysmon filtering using Logstash - Pablo Delgado](http://syspanda.com/index.php/2017/03/03/sysmon-filtering-using-logstash/)
      * [Sample sysmon events and the schema you can expect in Sysmon v6 - @williballenthin](https://gist.github.com/williballenthin/f693b1c2f3d95cb8f8e17b5f7f26031d)
      * [Sysmon Woes, Elasticsearch and MITRE’s ATT&CK Matrix - Black Lantern Security](http://www.blacklanternsecurity.com/blog/2016/12/11/sysmon-woes-elasticsearch-and-mitres-attack-matrix/)
      * [Parsing Sysmon Events for IR Indicators - CrowdStrike](https://www.crowdstrike.com/blog/sysmon-2/)
      * [Detecting Advanced Threats with Sysmon, WEF and ElasticSearch - Joshua Lewis](https://joshuadlewis.blogspot.com/2014/10/advanced-threat-detection-with-sysmon_74.html)
      * [Sysinternals New Tool Sysmon (System Monitor) - Carlos Perez](http://www.darkoperator.com/blog/2014/8/8/sysinternals-sysmon)
      * [Putting attackers in hi vis jackets with sysmon - Adrian Shaw](https://labs.nettitude.com/blog/putting-attackers-in-hi-vis-jackets-with-sysmon/)
      * [Sample sysmon events and the schema you can expect in Sysmon v6 - @williballenthin](https://gist.github.com/williballenthin/f693b1c2f3d95cb8f8e17b5f7f26031d)
    * [Sysmon Github Projects](#sysmon_github_projects)
      * [Powershell Sysmon - GitHub - Carlos Perez](https://github.com/darkoperator/Posh-Sysmon)
      * [Sysmon queries - GitHub - James Habben](https://github.com/JamesHabben/sysmon-queries)
      * [Splunk TA for Sysmon - GitHub - @daveherrald](https://github.com/splunk/TA-microsoft-sysmon)
      * [SplunkMon cofiguration - GitHub - The Crypsis Group](https://github.com/crypsisgroup/Splunkmon)
      * [Desired State Configuration for Deploying/Maintaining Sysmon - GitHub - @AwfulyPrideful](https://github.com/NotAwful/Sysmon-DSC)



# General

## Sysmon Configuration

**@SwiftOnSecurity config**

Recommended.

Config will assist with bringing you up to speed in relation to critical process monitoring, network utilization, and so on. Note that the concept is to not log everything, but the most important items.

https://github.com/SwiftOnSecurity/sysmon-config

**Sysmon_config.xml**

Solid, detailed config. Probably one of the best ones out there in relation to completeness.

[MalwareArchaeology](https://www.malwarearchaeology.com/logging/)

**Sysmon-a.cfg**

Basic config that will monitor critical Windows process execution. Very basic, but a good config to get used to sysmon and how things operate.

[Blog post by blacklanternsecurity](http://www.blacklanternsecurity.com/blog/2016/12/11/sysmon-woes-elasticsearch-and-mitres-attack-matrix/)

**Sysmon-b.cfg**

Crypsis Group published config and PDF. Fairly detailed list of excludes that should assist with understanding how they work and get a configuration started.

[Crypsis Group Config](https://github.com/crypsisgroup/Splunkmon/edit/master/sysmon.cfg)

[Crypsis Group PDF](http://www.crypsisgroup.com/images/site/CG_WhitePaper_Splunkmon_1216.pdf)

**Sysmon-c.cfg**

Great configuration to understand excludes and contains.

[Decent Security Config](https://decentsecurity.com/enterprise/#/sysmon-enterprise-configuration/)

**Sysmon-d.cfg**

Solid blog post related to getting started with Sysmon. Config is nicely laid out and easy to understand.

[909Research Blog](http://909research.com/sysmon-the-best-free-windows-monitoring-tool-you-arent-using/)

**Sysmon-e.cfg**

Config is specific but it provides a good foundation for capturing a lot of specific data.

https://github.com/Prevenity/sysmon

(Translated comments to english)

**Sysmoncfg_v2|31.xml**

Related material from Splunking the Endpoint .conf talk by James Brodsky and Dimitri McKay.

[Splunking the Endpoint - Files from presentation](https://splunk.app.box.com/v/splunking-the-endpoint)

Configs are optimized for Splunk.

**Additional configs**

Configs are updated frequently --

[SwiftOnSecurity Fork by Ion-Storm](https://github.com/ion-storm/sysmon-config/blob/master/sysmonconfig-export.xml)

Server Config: https://gist.github.com/Neo23x0/a4b4af9481e01e749409

Client config: https://gist.github.com/Neo23x0/f56bea38d95040b70cf5
