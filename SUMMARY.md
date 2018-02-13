# **<p align="center"><a href="https://www.federacy.org/">Federacy</a></p>**
*<p align="center">An open source, decentralized platform for security research and vulnerability management</P>*
<br>

## Table of Contents

 1. **<a name="intro1" href="#1intro">Introduction</a>**
 2. **<a name="summary2" href="#2summary">Summary</a>**
 
    2.1 <a name="problems2.1" href="#2.1problems">Problems</a>
    
    2.2 <a name="solutions2.2" href="#2.2solutions">Solutions</a>
    
 3. **<a name="problems3" href="#3problems">Problems</a>**
 
    3.1 <a name="security3.1" href="#3.1security">Security research is vastly underfunded</a>
    
    
      &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;3.1.1. <a name="ubiquity3.1.1" href="#3.1.1ubiquity">Ubiquity and freeloaders</a>
    
      &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;3.1.2. <a name="research3.1.2" href="#3.1.2research">Research vs. development</a>
    
      &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;3.1.3. <a name="responsible3.1.3" href="#3.1.3responsible">Responsible disclosure is not responsible</a>
      
      
    3.2. <a name="centralized3.2" href="#3.2centralized">Centralized vulnerability ecosystem is inefficient and inaccurate</a>
    
       
      &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;3.2.1. <a name="identifiers3.2.1" href="#3.2.1identifiers">Identifiers</a>
       
      &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;3.2.2. <a name="coverage3.2.2" href="#3.2.2coverage">Coverage gap</a>
       
      &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;3.2.3. <a name="tiered3.2.3" href="#3.2.3tiered">Tiered coverage</a>
       
      &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;3.2.4. <a name="structure3.2.4" href="#3.2.4structure">Structure and communication delays<a/>
       
      &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;3.2.5. <a name="distributed3.2.5" href="#3.2.5distributed">Distributed Weakness Filing and Automation Working Group</a>
       
      &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;3.2.6. <a name="collaboration3.2.6" href="#3.2.6collaboration">Collaboration and dispute resolution</a>
      
      &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;3.2.7. <a name="references3.2.7" href="#3.2.7references">References and artifacts</a>
       
      &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;3.2.8. <a name="subjective3.2.8" href="#3.2.8subjective">Subjective ratings</a>
       
      &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;3.2.9. <a name="public3.2.9" href="#3.2.9public">Public repository</a>
      
      
  4. **<a name="solutions4" href="#4solutions">Solutions</a>**
  
     4.1. <a name="anewp4.1" href="#4.1anewp">A new protocol</a>
  
     4.2. <a name="anewr4.2" href="#4.2anewr">A new repository</a>
  
     4.3. <a name="anewd4.3" href="#4.3anewd">A new dApp</a>
  
     4.4. <a name="anewe4.4" href="#4.4anewe">A new economy</a>
  
     4.5. <a name="anewf4.5" href="#4.5anewf">A new foundation</a>
     
     <br>
     <br>


## <p align="center"><a name="1intro" href="#intro1">1.</a> Introduction</p>

_<p align="center">A federacy to secure the Internet</p>_ 

<br>

This project is high risk. It’s success is predicated on shifting the security ecosystem from reliance on a government-controlled protocol/database to ones that are open, public, and managed by the collective Internet.

Every company is at risk of being compromised because our existing security infrastructure is failing.  The core vulnerability protocol and database (CVE/NVD) that the current security ecosystem are built upon are funded and controlled by the United States Department of Homeland Security. Incomplete and inaccurate data, underfunding, and poor governance structure, has severely hindered progress on essential security tooling. Further, core Internet infrastructure, and the open source software that almost every company in the world relies upon, lacks the financial framework to adequately incentivize security research. 

Federacy is developer infrastructure for security research and vulnerability management. It is a new, open protocol and a decentralized repository for vulnerabilities that is available for all developers to leverage.

The first dApp built on top of this infrastructure will allow companies to directly fund security research for the open source software they depend on.  We expect other developers to build dApps that will include vulnerability scanning, policy engines, asset controls, and more robust tooling for secure, self-healing distributed systems. 

<br>
<br>

## <p align="center"> <a name="2summary" href="#summary2">2.</a> Summary</p>

### <a name="2.1problems" href="#problems2.1">2.1</a> Problems

* Security research within core Internet infrastructure and open source software is vastly underfunded.
* The existing, centralized vulnerability ecosystem is inefficient and inaccurate.
* Tooling required for secure, self-healing, containerized, distributed systems requires a shared, open source protocol and infrastructure.


### <a name="2.2solutions" href="#solutions2.2">2.2</a> Solutions

* A new **protocol** for communicating reports, ratings and remediations, linked by an immediately-available identifier.
* A new, **decentralized, vulnerability repository** built on a community-owned blockchain that is resilient, trustworthy and immutable—and by the nature of incentivized participation, significantly more robust. 
* A new **dApp** with **transparent, auditable, and trustless smart contracts** to facilitate and incentivize security research and collaboration.
* A new **token** and **inflation-driven economy** to directly fund researchers and enable companies to support the open source software on which they depend on.
* A new, **nonprofit foundation** governed by all stakeholders with the sole mission of providing open source software with additional resources to help secure the Internet.
<br>

## <p align="center"><a name="3problems" href="#problems3">3.</a> Problems </p>

### <a name="3.1security" href="#security3.1" >3.1.</a> Security research is vastly underfunded

Every major company in the world uses open source software. Cloud computing and containerization has made it nearly ubiquitous. From Kubernetes and Docker to Nginx and the Linux kernel, open source software exists in nearly every software stack and serves as a building block for more efficient innovation.

<br> 

### <a name="3.1.1ubiquity" href="#ubiquity3.1.1">3.1.1.</a> Ubiquity and freeloaders

According to Gartner, open source software will be included in mission-critical applications within 99% of Global 2000 enterprises by the end of 2016 <sup name="a1">[[1]](#f1)</sup>. In their analysis of software in M&A, Black Duck Software sees open source software comprising 20% - 50% of code they scan, and over 90% of code bases scanned contain undisclosed open source code <sup name="a2">[[2]](#f2)</sup>. 

We've made the collective assumption that if everyone uses open source software, it must be secure. Nothing could be further from the truth—as exhibited by breach after breach of major corporations and governments. Incidentally, the more people who use a piece of software, the more incentive there are for nefarious actors to exploit it. 

Despite the prevalence of open source software, many vulnerabilities within it go undiscovered and/or unreported. One of the primary reasons is that open source software lacks the organizational structure to support and adequately fund security research. Unreported vulnerabilities, known as zero days, are a grave problem— the depth of which was revealed in June 2017 when the CIA <sup name="a3">[[3]](#f3)</sup> and NSA <sup name="a4">[[4]](#f4)</sup> had their zero day stockpiles leaked, affirming that brokers, and nation-states alike, pay very large sums for unreported vulnerabilities. 

In contrast, open source security research and bug bounty programs do not pay well. For example: Heartbleed was a significant vulnerability in OpenSSL, software that powers encryption on the Internet. The security researcher that identified the vulnerability, Neel Mehta, was paid just $15K—though had he chosen to, could have sold it for millions.  At the time of Heartbleed, OpenSSL—which 17.5% of the encrypted websites on the Internet use<sup name="a5">[[5]](#f5)</sup>, was maintained by one full-time employee and volunteers on a $2K annual budget <sup name="a6">[[6]](#f6)</sup>.

<br>

### <a name="3.1.2research" href="#research3.1.2">3.1.2.</a> Research vs. development 

Security research and best practices are fundamentally different than authoring open source software and require a separate toolset, including linting, fuzzing, penetration testing, and manual introspection with an eye for potential vulnerabilities. 

Open source authors and project maintainers are often volunteers (or extremely underpaid), and have a myriad of demands for their already limited time/resources. Triaging and resolving vulnerability reports are frequently undesired burdens and as the means of vulnerability discovery advance the sheer number of reports will become too much work for a small team. When severe vulnerabilities reported by security researchers to widely-used, open source software providers, it can take many months before they are patched. One recent example is CVE-2017-0902 <sup name="a7">[[7]](#f7)</sup>, a  RubyGems RCE vulnerability that was formally reported five months prior to being patched (and discovered as early as two years prior). 

During the time between report and patch, any number of bad actors (the reporter, RubyGems maintainer, or any recipient of the report) could profit-seek, selling the vulnerability to brokers or exploiting it themselves. Likewise, other researchers may find the same vulnerability, thereby proliferating its exploitation. 

<br>

### <a name="3.1.3responsible" href="#responsible3.1.3">3.1.3.</a> Responsible disclosure is not responsible

Traditionally, responsible disclosure has involved delaying publicizing a vulnerability until it has been patched, in order to reduce the likelihood of a malicious actor using public information to exploit the vulnerability. During this period of silence, no one using the vulnerable software knows they are vulnerable. This hampers other actions one could take to mitigate or remediate the issue without a patch, such as configuration changes or by limiting access.

The problems with this approach are: 

1. Users of the software, and their customers, are vulnerable.
2. It presumes no one else will discover the vulnerability.
3. The researcher, the vendor, and everyone in between, have the opportunity to profit-seek.

This is exemplified but the recently revealed processor vulnerabilities known as Meltdown and Spectre.  In early 2018, the revealation of these vulnerabilities shook the industry since they impacted almost every current processor. These vulnerabilities were initially warned about as early as in May 1995, with a paper funded by the NSA <sup name="a8">[[8]](#f8)</sup>. 

Between June and December 2017, four different researchers and groups discovered and reported the issues to Intel. Intel attempted to coordinate a disclosure for January 9th.  However, public news reports based on commits to the Linux kernel and messages to the mailing list, prompted ending the embargo early (on January 3rd) before patches became available for many operating systems. 

Only on January 4th was a CVE created, and it wasn't until the 5th that NVD analyzed the vulnerability, assigning a rating of 5.6 <sup name="a9">[[9]](#f9)</sup>, despite Intel itself rating it an 8.2 <sup name="a10">[[10]](#f10)</sup>. This is not an isolated case, and while research on these topics is opaque, RAND and Harvard's Belfer Center for Science and International Affairs, found between 5.7% <sup name="a11">[[11]](#f11)</sup> and 21% <sup name="a12">[[12]](#f12)</sup> vulnerability re-discovery rate. 

The existing disclosure policy favors companies and software vendors too heavily, which unnecessarily puts consumers and citizens at risk. Instead, we advocate for a real-time, public, vulnerability database. This will allow companies to adequately evaluate how vulnerable they are and take corrective actions, including the funding of research and remediation of the vulnerabilities impacting them. Even when CVE and NVD hold back reports and information, the rest of the community moves forward, sometimes utilizing the CVE number as a reference, while most automated security scanners remain blind.

<br> 

### <a name="3.2centralized" href="#centralized3.2">3.2.</a> Centralized vulnerability ecosystem is inefficient and inaccurate

Kubernetes, Docker, and self-healing, distributed systems have made immediate, automated patching possible. However, without an accurate, real-time data source for vulnerabilities, security posture cannot realistically be made a primary aspect of system health.

![CVE/NVD Vulnerability Reporting Flow](/images/vulnerability_reporting_flow.png)

Our existing centralized vulnerability ecosystem for reporting, rating, and remediating vulnerabilities is unnecessarily inefficient <sup name="a13">[[13]](#f13)</sup> and inaccurate <sup name="a14">[[14]](#f14)</sup>. In July, the Energy and Commerce Committee of the US House of Representatives sent letters to the Department of Homeland Security and MITRE regarding the performance of the "critical cyber database" <sup name="a15">[[15]](#f15)</sup>. 

Common Vulnerabilities and Exposures (CVE) is a dictionary of software vulnerabilities created in 1999 by the MITRE corporation. CVE numbers are issued as an identifier for each unique vulnerability reported to allow researchers, developers, companies to track and discuss them. 

The NVD is a superset of the CVE database, operated by the United States Department of Commerce's National Institute of Standards and Technology (NIST). It adds metadata to CVE entries regarding products impacted, and rates the severity of the vulnerability based on several factors. 

Both the CVE and NVD are funded by the United States Department of Homeland Security, and despite consistent efforts by many members of both entities’ governing boards to improve them, it is our belief that neither entity can keep up with the pace that security ecosystem requires.

<br> 

### <a name="3.2.1identifiers" href="#identifiers3.2.1">3.2.1.</a> Identifiers


> Over time, it has become clear that the days of the "One Vulnerability
> ID to Rule Them All" were coming to a close and we need to start
> planning for that change. As I've covered above, one of the key
> observations we've made has been the growing need for multiple
> vulnerability identifiers and databases that serve different
> audiences, support diverse business practices, and operate at
> different characteristic rates <sup name="a16">[[16]](#f16)</sup>.
 
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; *-Allen Householder, Senior Vulnerability & Incident Researcher, CERT Coordination Center* 

MITRE and CNAs perform deduplication and some level of validation on CVE reports.  This vetting process takes time <sup name="a17">[[17]](#f17)</sup> and creates a lag between when a report is made and when it becomes publicly available. This analysis can include factors counter to public interest.  For example, when a vendor is no longer supporting a product, it can lead to reports being rejected, and never being issued identifiers. This human-driven vetting process is the reason why the NVD/CVE system is so slow. 

The concept of separating the **identifier, initial report,** and **supporting documentation** is not a new one. On September 3rd, 2014, Will Dormann released the results of automated, SSL, man-in-the-middle research <sup name="a18">[[18]](#f18)</sup>, utilizing CERT's Basic Fuzzing Framework <sup name="a19">[[19]](#f19)</sup>. In total, there were over 20,500 vulnerabilities, and only 1,384 of them received CVE-IDs <sup name="a20">[[20]](#f20)</sup>. Further coordination was through a single CERT Vulnerability Note <sup name="a21">[[21]](#f21)</sup> and spreadsheet <sup name="a22">[[22]](#f22)</sup>. 

> We, of course, were not alone in discovering the effectiveness of
> fuzzing and other kinds of automated testing to find new
> vulnerabilities. The end result was that, from our perspective, the
> volume and arrival rate of incoming cases was unconstrained, while our
> capacity to produce documents could only react at a much slower rate
> (hiring and training wind up being on the critical path) <sup name="a23">[[20]](#f23)</sup>.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; *-Allen Householder, Senior Vulnerability & Incident Researcher, CERT Coordination Center* 

<br> 

### <a name="3.2.2coverage" href="#coverage3.2.2">3.2.2.</a> Coverage gap

Risk Based Security, one of the leading private vulnerability databases, has estimated that less than 61% of all discovered vulnerabilities are formally reported to MITRE.  However, known vulnerabilities are increasing, with Q3 2017 being 38% higher than the same period in 2016 <sup name="a24">[[24]](#f24)</sup>.

![Discovered vulnerabilities formally reported to MITRE](/images/rbs_known_vulnerabilities.png)
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; *-Risk Based Security* 

This coverage gap is a major problem. In May of 2016, US-CERT issued its first alert for SAP applications <sup name="a25">[[25]](#f25)</sup>, and dozens of organizations were impacted by attackers utilizing a vulnerability that was patched in 2010. However, while there was a patch, and the vulnerability’s presence was noted in several other vulnerability databases, a CVE-ID was not assigned until 2016 <sup name="a26">[[26]](#f26)</sup>, despite SAP being a Tier 1 (must cover) organization. 

One of the factors contributing to this coverage gap is that CVE/NVD are an authoritative system with administration driven by humans who analyze and process submissions. In contrast, China's National Vulnerability Database (CNNVD) pulls information from CVE/NVD and many other public sources. Consequently, China's VDB is more comprehensive, and more timely: 

* average time between disclosure and database inclusion (13 days versus 33 days) <sup name="a27">[[27]](#f27)</sup>
* 1,746 CVEs are absent in the NVD, but present in CNNVD; hundreds are reported first by CNNVD <sup name="a28">[[28]](#f28)</sup>
* three-quarters of vulnerabilities are publicly reported online before NVD publication. <sup name="a28">[[28]](#f28)</sup>

It is also likely that coordination with China's Ministry of State Security and Advanced Persistent Threat (APT) teams means that vulnerabilities being actively exploited have a delayed release <sup name="a29">[[29]](#f29)</sup>, which effectively means lack of vulnerability disclosure is being used as an offensive capability.

<br> 

### <a name="3.2.3tiered" href="#tiered3.2.3">3.2.3.</a> Tiered coverage

Another factor that contributes to the coverage gap is that MITRE uses a tiered approach, ranging from "must cover," to "must not cover." This results in many products not being eligible for identifiers, and there has been much disagreement about tier— with MITRE itself acknowledging that they do not have a good way to prioritize the tens of thousands of Linux packages <sup name="a30">[[30]](#f30)</sup>.  Libraries like ImageMagick, FFmpeg, and PCRE can impact thousands of vendors, companies and are tier 4, "May Not Cover." These products are given the lowest priority.

<br> 

### <a name="3.2.4structure" href="#structure3.2.4">3.2.4.</a> Structure and communication delays

![CVE Submission Process](/images/rf_submission_process.png)
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; *-Recorded Future, Inc* 

The rules and guidelines for communication between parties involved in the vulnerability disclosure process are very lax. Even the newest drafts of the CNA rules allow 24 hours to update upstream CNAs <sup name="a31">[[31]](#f31)</sup>. CNA's will sometimes reject reports because they are out of scope or for a product that is no longer supported <sup name="a32">[[32]](#f32)</sup>. Researchers frequently have trouble getting CVE-IDs issued in a timely manner <sup name="a33">[[33]](#f33)</sup>.

When the CVE database has been updated, NIST will analyze the information <sup name="a34">[[34]](#f34)</sup> for roughly 15 minutes, which they aim to complete within two business days, excluding federal holidays <sup name="a35">[[35]](#f35)</sup>. The review is primarily of the prose description in the CVE <sup name="a36">[[36]](#f36)</sup> and references from which NVD creates metadata regarding products and versions impacted (CPEs) along with the type of vulnerability (CWE). 

Between the time a vendor or researcher reserves a CVE and when they publish information to MITRE, the CVE remains in a "RESERVED" state and will not be analyzed for NVD <sup name="a37">[[37]](#f37)</sup>. Consequently, most vulnerability scanners will not detect it, despite that there is often public information about the vulnerability; ranging from further research, to mitigation and remediation advice. 

As of December 18th, 2016, 47% of all 10,137 CVEs were in a RESERVED state <sup name="a38">[[38]](#f38)</sup>. This can have a profound impact not just on automated vulnerability scanning, but security researchers themselves— it essentially means that CVE is not a primary source for up-to-date vulnerability information <sup name="a39">[[39]](#f39)</sup>.

<br> 

### <a name="3.2.5distributed" href="#distributed3.2.5">3.2.5.</a> Distributed Weakness Filing and Automation Working Group

In an effort to keep pace, the MITRE board has opted for a federated strategy for CNAs. One of the new CNAs, the Distributed Weakness Filing (DWF), is designated for all open source projects that currently do not have an appointed CNA. 

DWF was created by Kurt Sefried, a CVE board member and Red Hat employee, due to frustration with MITRE not issuing CVEs in a timely manner (or issuing them at all) nor communicating <sup name="a40">[[40]](#f40)</sup>. It is a new take on a CNA: Red Hat uses Bugzilla <sup name="a41">[[41]](#f41)</sup>; DWF uses a Github <sup name="a42">[[42]](#f42)</sup> and Google Spreadsheet <sup name="a43">[[43]](#f43)</sup> driven approach that is being piloted by the CVE Board's Automation Working Group <sup name="a44">[[44]](#f44)</sup>.

This is a huge step forward and provides open source projects a better experience than going directly through MITRE.  However, even with this approach, there are cracks around the edges. DWF sub-CNAs forking the repo is causing issues <sup name="a45">[[45]](#f45)</sup>, the git history is sparse <sup name="a46">[[46]](#f46)</sup>, and the spreadsheet's history is not public <sup name="a47">[[47]](#f47)</sup>.

<br> 

### <a name="3.2.6collaboration" href="#collaboration3.2.6">3.2.6.</a> Collaboration and dispute resolution

> Historically there has been a need for slower, consistently
> high-quality, authoritative vulnerability records, trading off higher
> latency for lower noise. Deconfliction of duplicate records happens
> before issuance, and reconciliation of errors can be difficult. To
> date, this practice is the ideal that many VDBs have strived for.
> Those VDBs remain a valuable resource in the defense of systems and
> networks around the globe.   Yet there is a different ideal, just as
> valid: one in which vulnerability IDs are assigned quickly, possibly
> non-authoritatively, and based on reports of variable quality. This
> process looks more like "issue, then deconflict". For this new process
> to work well, post-hoc reconciliation needs to be easier <sup name="a48">[[48]](#f48)</sup>.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; *-Allen Householder, Senior Vulnerability & Incident Researcher, CERT Coordination Center* 

When a CVE is issued by a CNA, be it a root CNA, a sub-CNA, or MITRE, it contains at least a description, a reference URL, and may also include the products impacted, and the type of vulnerability. Currently, we expect that the reporter will have full knowledge of a vulnerability when it is reported. 

However, many different stakeholders may have information to contribute. For example, Red Hat, OpenSuSE, and NVD may all have different views on the rating of a vulnerability, while a package maintainer may know what versions of their software are impacted. This becomes even more significant when we consider a single vulnerability which impacts hundreds of vendors and projects, all of whom may want to contribute to the report. 

When a third party (another CNA, researcher, or vendor) wants to contribute, they currently must submit a web form to MITRE <sup name="a49">[[49]](#f49)</sup>. MITRE, or a root CNA, then resolves the conflict before updating the record. To get the rating, products impacted, or vulnerability type updated, one must email nvd@nist.gov <sup name="a50">[[50]](#f50)</sup>. In either case, it can take days to be updated and propagate. 

If a vendor wants to dispute a CVE report, they can contact MITRE, who will mark the CVE as "DISPUTED"; however, no further collaboration or dispute resolution occurs <sup name="a51">[[51]](#f51)</sup>. Consequently, there a public log of differing opinions about a vulnerability does not exist, and independent conflict resolution is not possible. This data is paramount to automated patching, as company policy should be based on whose opinion matters to them.  In the United States, CVE/NVD are integral to HIPAA and PCI DSS, but there are similar organizations around the world; China even has two. Likewise, companies should be able to follow the guidance of organizations they trust: specific security vendors and researchers.  

Art Manion is a senior member of the Vulnerability Analysis team in the CERT Program at the Software Engineering Institute (SEI), Carnegie Mellon University. He provided an example of how such a system could work to the CVE Board:

> CERT/CC publishes a vulnerability and writes the corresponding CVE 
> entry, submits via github, entry goes into CVE corpus and on to NVD.
> 
> Red Hat disagrees with any part of the entry and wants to make a
> change.  There's  a facility to add a comment to the entry saying: "On
> $date, Red Hat says:   The CVSS score is wrong, here are two new
> references, and the version info in the  description should be
> updated."  Depending on the nature of the comment,  DISPUTED status is
> set.
> 
> Assuming such a comment can be added with little or no friction (and 
> here is part of the business rules discussion, who can add comments, 
> with or without review?), CVE consumers now have new information.  The
> record hasn't been changed yet.  CERT/CC responds, Red Hat responds, 
> someone else throws in, and the public comment log has provided a path
> to allow convergence.  In this example, CERT/CC is a responsive CNA, 
> considers and agrees with the comments, and updates the CVE entry.
> 
> When reading the original CVE entry and decide I never listen to what 
> Red Hat says, I can ignore the comment.  If I think Red Hat is right,
> I  can act on the comment even before the entry is converged/updated.
> 
> And if there's no convergence, maybe some other rules or review come 
> into play, and a CNA upstream from CERT/CC decides to make changes. 
> Or  the comment log sits there, documenting the dispute <sup name="a52">[[52]](#f52)</sup>.

<br>

### <a name="3.2.7references" href="#references3.2.7">3.2.7.</a> References and artifacts

Submitting a CVE requires a reference URL with details about the vulnerability beyond the description, even if the description contains all necessary or known information. MITRE does not mirror nor archive these references; it does not intend to do proactive reference maintenance <sup name="a54">[[53]](#f53)</sup>, so an artifact and reference repository is likely out of scope. The limited reference maintenance MITRE is willing to do relates to when a whole domain has changed, as occurred recently with over 20,000 references in IBM's X-Force database. This is less than ideal because the vulnerability database should be comprehensive—all artifacts necessary for research and analysis should be included within it. A reference URL should be optional, and the report should ideally include relevant information from the reference URL. A recent proposal by Kurt Seifreid to resolve part of this issue by amending the rules to allow a self-referencing URL has received pushback <sup name="a54">[[54]](#f54)</sup>. 

<br> 

### <a name="3.2.8subjective" href="#subjective3.2.8">3.2.8.</a> Subjective Ratings

Vulnerability ratings allow both people and security software, such as scanners, to understand the severity of a vulnerability.  

![CVSSv3 Rating Rubric](/images/cvss3_rating_rubric_header.png)

![CVSSv3 Rating Rubric](/images/cvss3_rating_rubric.png)

The rubric above is clear, but subjective. Ratings are primarily done on behalf of NIST's NVD (National Vulnerability Database) or operating system vendors like Red Hat and Ubuntu, who often draw differing conclusions on the final rating of a vulnerability. These ratings also dictate the requirements and timeline for remediation under PCI DSS and HIPAA compliance regulations. If ratings are inaccurate, a significant vulnerability may go unpatched forever. 

<br>

### <a name="3.2.9public" href="#public3.2.9">3.2.9.</a> Public Repository

MITRE and NIST handle an important role in the ecosystem since their analyses drive the PCI DSS and HIPAA processes. However,  we believe the CVE/NVD system has severe shortcomings as a technical solution to the challenges inherent in distributed vulnerability research.

These roles can be separated and a real-time, public vulnerability database encompassing more contributor with more information can be created. Further, the role of gatekeeper to the public vulnerability ecosystem should be played by a nonprofit organization with an equitable governance structure so that significant decisions can be made fairly.

<br>
<br>

## <p align="center"><a name="4solutions" href="#solutions4">4.</a> Solutions </a></p>

> <p align="center"> Blockchain would solve a pile of these problems </p>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; *-Kurt Seifried, CVE Board member <sup name="a55">[[55]](#f55)</sup>*

![Federacy Blockchain as a Vulnerability Database](/images/blockchain_rubric.png)

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; *-Rubric source: Allen Householder <sup name="a56">[[56]](#f56)</sup>*

<br>

### <a name="4.1anewp" href="#anewp4.1">4.1.</a> A New Protocol
------

*<p align="center">Specification for communicating reports, ratings, and remediations driven by an immediately available identifier</p>*

<br>

A new protocol for communicating about vulnerabilities will enable collation of research; consensus about impact and surface area; incentivisation for all contributors and stakeholders; thereby, automation. 

It will be driven by an immediately available identifier—specifically, the address of the smart contract representing the contribution.  It will be based on the Linux Foundation's *Software Package Data Exchange (SPDX) <sup name="a57">[[57]](#f57)</sup>*, NYU's *The Update Framework (TUF) <sup name="a58">[[58]](#f58)</sup>*, and the Forum of Incident Response and Security Teams' (FIRST) *Vulnerability Reporting and Data eXchange SIG (VRDX-SIG) <sup name="a59">[[59]](#f59)</sup>*, specifications. 

The protocol enables more timely and accurate propagation as new information becomes publicly known about vulnerabilities. In combination with self-healing, containerized, distributed systems, this permits immediate, automatic patching and much more effective visibility into the real-time status of security posture. 

This protocol will be the foundation for an ecosystem that will include new, distributed industries and functionality.  This also entails asset management, access restriction using a policy engine, bill of materials generation, vulnerability scanning, and license assurances. 

<br>

### <a name="4.2anewr" href="#anewr4.2">4.2.</a> A New Repository
------

*<p align="center">Decentralized vulnerability datastore built on a community-owned blockchain</p>*

<br>

Federacy is a public vulnerability repository. Due to the nature and value of this data, a decentralized, immutable store (blockchain) is required because:  

1. it **should be** *publicly verifiable*.
2. it **should be** *always available*.
3. collaboration **should not** require trust.
4. it **should not** depend on or be governed by a central authority.

Double permissionless, distributed ledgers provide the means for the larger system to not rely on any single stakeholder, including Federacy. 

They ensure public verifiability, meaning that no single organization can alter history, and all transactions are trustworthy. This is required by the smart contracts and tokens, which power the incentivization process. 

<br>

### <a name="4.3anewd" href="#anewd4.3">4.3.</a> A New dApp
------

*<p align="center">Transparent, auditable, and trustless smart contracts
to facilitate and incentivize security research</p>*

<br>

Smart contracts allow untrusted third parties to work together toward a common goal using transparent terms. They enable every contributor along the way—from vulnerability discoverer to remediator—to be compensated and attributed for their work, in a publicly verifiable way.

**Report**

To encourage distributed, collaborative research, a staking system will be used to rewards timely, accurate vulnerability research that includes: 

* rating
* type
* software impacted
* versions impacted 
* other assets impacted (containers, images)

When researchers submit a new report, a smart contract is created representing that report. Subsequent contributions of information will reference the contract address, and if accurate, will result in compensation. The veracity of each piece of information is integral.  For instance, if a major rating factor is defined incorrectly, it could ultimately delay a pertinent patch by months. 

Reports and contributions require a small transaction fee to be paid, which disincentivizes bad actors, while incentivizing accuracy.

**Remediate**

When a contributor has written a patch for a vulnerability, they create a resolution identifier and include it in the commit message. When the upstream repo merges their patch, it will trigger a distribution event wherein all reporters, contributors, remediators, and the upstream maintainer are rewarded. 

**Fund**

In addition to enabling blanket support of all security research for a specific software, smart contracts allow any interested party—company, researcher, or project maintainer—to contribute resources directly to any step of the research and remediation process.

<br>

### <a name="4.4anewe" href="#anewe4.4">4.4.</a> A New Economy
------

*<p align="center">Rewards researchers and enables companies to support open source software</p>*

<br>

**Researchers earn tokens by:**

1. finding and reporting vulnerabilities
2. reviewing and rating vulnerabilities
3. submitting patches for vulnerabilities

**Companies buy tokens to:**

1. directly support research into software projects on which they rely
2. fund bounties for a bug bounty and vulnerability program covering their own software
3. hold in support of all open source security research
4. request scans and bill of materials generation for specific packages and images
5. utilize the services of third-party products built on top of Federacy

An **inflation-driven economy** directly funds security research for top open source projects by continuously allocating new tokens to smart contracts representing these projects. Along with contributions from companies and other stakeholders, these funds provide the basis for compensating researchers and project maintainers. 

This inflation mechanism aligns interests, enabling companies to directly support security research for the open source software on which they rely. And in turns, researchers and stakeholders would be adequately rewarded for their contributions. 

Security research is time-sensitive and intensive, but not geographically exclusive, which means that it is accessible to billions of people in the world. Researchers should be able to earn livable wages, thereby creating a pool of researchers that did not previously exist—we envision this pool growing to be the largest pool of security researchers ever assembled.

A token is required for incentivization which allows contributors to focus on their specialties and areas of interest while remaining anonymous if they so choose. While the token does not require widespread buy-in to be functional, we anticipate self-interest to motivate strong network effects within the ecosystem. The value of compensation (tokens) increases as adoption increases, and early contributors stand to benefit significantly for early participation. 

<br>

### <a name="4.5anewf" href="#anewf4.5">4.5.</a> A New Foundation
------

*<p align="center">Nonprofit, open source, community-driven</p>*

<br>

Federacy will move decision-making outward to the stakeholders closest to the problems while allowing everyone a voice and an opportunity to be rewarded for their contributions. Our goal is to make Federacy the de facto infrastructure for vulnerability management; so accordingly, it must be open and transparently managed by all stakeholders in the ecosystem. 

<br>
<br>
------
<br>
<br>
<b name="f1"><a href="#a1">[1]</a></b>  Driver, Mark. “<a href="https://www.gartner.com/doc/2158016/drivers-incentives-wide-adoption-opensource">Drivers and Incentives for the Wide Adoption of Open-Source Software.</a>” Gartner, Inc., 13 Sept. 2012 

<b name="f2"><a href="#a2">[2]</a></b> “<a href="http://www.blackducksoftware.com/files/webmedia/_webinars/08-27-13_SAP_M-A.pdf">Open Source Software and the Impact on Mergers & Acquisitions.</a>” Black Duck Software 

<b name="f3"><a href="#a3">[3]</a></b> Shane, Scott, et al. “<a href="http://www.nytimes.com/2017/03/07/world/europe/wikileaks-cia-hacking.html">WikiLeaks Releases Trove of Alleged C.I.A. Hacking Documents.</a>” The New York Times, The New York Times, 7 Mar. 2017

<b name="f4"><a href="#a4">[4]</a></b> Nakashima, Ellen. “<a href="http://www.washingtonpost.com/world/national-security/powerful-nsa-hacking-tools-have-been-revealed-online/2016/08/16/bce4f974-63c7-11e6-96c0-37533479f3f5_story.html">Powerful NSA Hacking Tools Have Been Revealed Online.</a>” The Washington Post, 16 Aug. 2016.

<b name="f5"><a href="#a5">[5]</a></b> Mutton, Paul. “<a href="http://news.netcraft.com/archives/2014/04/08/half-a-million-widely-trusted-websites-vulnerable-to-heartbleed-bug.html">Half a Million Widely Trusted Websites Vulnerable to Heartbleed Bug.</a>” Half a Million Widely Trusted Websites Vulnerable to Heartbleed Bug | Netcraft, Netcraft, 8 Apr. 2014.

<b name="f6"><a href="#a6">[6]</a></b> Marquess, Steve. “<a href="http://veridicalsystems.com/blog/of-money-responsibility-and-pride/">Of Money, Responsibility, and Pride.</a>” Speeds and Feeds, 12 Apr. 2014.

<b name="f7"><a href="#a7">[7]</a></b> "<a href="https://nvd.nist.gov/vuln/detail/CVE-2017-0902">CVE-2017-0902</a>", National Vulnerability Database, 31 Aug. 2017.

<b name="f8"><a href="#a8">[8]</a></b> Sibert, Olin, et al. “<a href="http://doi.ieeecomputersociety.org/10.1109/SECPRI.1995.398934">The Intel 80x86 Processor Architecture: Pitfalls for Secure Systems.</a>” 1995

<b name="f9"><a href="#a9">[9]</a></b>  "<a href="https://nvd.nist.gov/vuln/detail/CVE-2017-5715">CVE-2017-5715</a>", National Vulnerability Database, 4 Jan. 2018.

<b name="f10"><a href="#a10">[10]</a></b> “<a href="https://security-center.intel.com/advisory.aspx?intelid=INTEL-SA-00088&languageid=en-fr">INTEL-SA-00088: Speculative Execution and Indirect Branch Prediction Side Channel Analysis Method.</a>” Product Security Center, Intel, 3 Jan. 2018

<b name="f11"><a href="#a11">[11]</a></b> Ablon, Lillian, and Timothy Bogart. “<a href="https://www.rand.org/pubs/research_reports/RR1751.html">The Life and Times of Zero-Day Software Vulnerabilities.</a>” RAND Corporation, 9 Mar. 2017

<b name="f12"><a href="#a12">[12]</a></b> Schneier, Bruce, et al. “<a href="https://www.belfercenter.org/publication/taking-stock-estimating-vulnerability-rediscovery">Taking Stock: Estimating Vulnerability Rediscovery | Belfer Center for Science and International Affairs.</a>” Harvard Kennedy School Belfer Center for Science and International Affairs, July 2017

<b name="f13"><a href="#a13">[13]</a></b> Seifried, Kurt. “<a href="https://cve.mitre.org/data/board/archives/2016-03/msg00002.html">Concerns about CVE Coverage Shrinking.</a>” CVE Editorial Board, 4 Mar. 2016.

<b name="f14"><a href="#a14">[14]</a></b> Stone, Ashley. “<a href="https://blog.blackducksoftware.com/how-accurate-is-cvss-scoring">How Accurate Is CVSS Scoring?,/a>” Black Duck Software Blog, 9 June 2017.

<b name="f15"><a href="#a15">[15]</a></b> Walden, Greg. “<a href="http://energycommerce.house.gov/news/letter/letters-dhs-and-mitre-regarding-performance-critical-cyber-database">Letters to DHS and MITRE Regarding Performance of Critical Cyber Database.</a>” Energy and Commerce Committee, US House of Representatives, 6 July 2017.

<b name="f16"><a href="#a16">[16]</a></b> Householder, Allen. “<a href="https://insights.sei.cmu.edu/cert/2016/03/vulnerability-ids-fast-and-slow.html">Vulnerability IDs, Fast and Slow.</a>” CERT/CC Blog, Software Engineering Institute, Carnegie Mellon University, 11 Mar. 2016.

<b name="f17"><a href="#a17">[17]</a></b> Wassermann, Garret. “<a href="https://vuls.cert.org/confluence/display/Wiki/CVE+IDs+and+How+to+Obtain+Them#CVEIDsandHowtoObtainThem-HowdoIgetaCVEdictionaryentryupdated?">CVE IDs and How to Obtain Them.</a>” Vulnerability Analysis Wiki, CERT Coordination Center (CERT/CC), 3 May 2017.

<b name="f18"><a href="#a18">[18]</a></b> Dormann, Will. “<a href="https://insights.sei.cmu.edu/cert/2014/09/-finding-android-ssl-vulnerabilities-with-cert-tapioca.html">Finding Android SSL Vulnerabilities with CERT Tapioca.</a>” CERT/CC Blog, Software Engineering Institute, Carnegie Mellon University, 3 Sept. 2014.

<b name="f19"><a href="#a19">[19]</a></b> “<a href="https://github.com/CERTCC-Vulnerability-Analysis/certfuzz">Certfuzz Project.</a>” GitHub, 17 Dec. 2016.

<b name="f20"><a href="#a20">[20]</a></b> Martin, Brian. “<a href="https://blog.osvdb.org/category/vulnerability-statistics/">The Duality of Expertise: Microsoft.</a>” OSVDB, 20 Mar. 2017

<b name="f21"><a href="#a21">[21]</a></b> “<a href="https://www.kb.cert.org/vuls/id/582497">Vulnerability Note VU#582497.</a>” Vulnerability Notes Database, Software Engineering Institute, Carnegie Mellon University, 8 Nov. 2016.

<b name="f22"><a href="#a22">[22]</a></b> Will Dormann. "<a href="https://docs.google.com/spreadsheets/d/1t5GXwjw82SyunALVJb2w0zi3FoLRIkfGPc7AMjRF0r4">Android Apps that fail to validate SSL.</a>", Google Sheets. 

<b name="f23"><a href="#a23">[23]</a></b> Householder, Allen. “<a href="https://insights.sei.cmu.edu/cert/2016/03/vulnerability-ids-fast-and-slow.html">Vulnerability IDs, Fast and Slow.</a>” CERT/CC Blog, Software Engineering Institute, Carnegie Mellon University, 11 Mar. 2016.

<b name="f24"><a href="#a24">[24]</a></b> “<a href="https://www.riskbasedsecurity.com/2017/11/no-shock-worst-year-for-vulnerabilities-already-only-through-q3-2017/">Worst Year For Vulnerabilities Already – Only Through Q3 2017.</a>” Risk Based Security, 14 Nov. 2017.

<b name="f25"><a href="#a25">[25]</a></b> "<a href="https://www.us-cert.gov/ncas/alerts/TA16-132A">Alert TA16-132A: Exploitation of SAP Business Applications.</a>" US-CERT, Department of Homeland Security, 11 May 2016.

<b name="f26"><a href="#a26">[26]</a></b>  "<a href="http://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2010-5326">CVE-2010-5326</a>", National Vulnerability Database, 12 May. 2016.

<b name="f27"><a href="#a27">[27]</a></b> Ladd, Bill. “<a href="https://www.recordedfuture.com/chinese-vulnerability-reporting">The Dragon Is Winning: U.S. Lags Behind Chinese Vulnerability Reporting.</a>” Recorded Future, 18 Oct. 2017.

<b name="f28"><a href="#a28">[28]</a></b> Ladd, Bill. “<a href="https://www.recordedfuture.com/vulnerability-disclosure-delay/">The Race Between Security Professionals and Adversaries.</a>” Recorded Future, 12 June 2017.

<b name="f29"><a href="#a29">[29]</a></b> Moriuchi, Priscilla, and Bill Ladd. “<a href="https://www.recordedfuture.com/chinese-mss-vulnerability-influence/">China's Ministry of State Security Likely Influences National Network Vulnerability Publications.</a>” Recorded Future, 17 Nov. 2017.

<b name="f30"><a href="#a30">[30]</a></b> Evans, Jonathan L. “<a href="https://cve.mitre.org/data/board/archives/2016-01/msg00015.html">Updating the Products and Sources List.</a>” Editorial Board Mailing List, MITRE Corporation, 7 Jan. 2016.

<b name="f31"><a href="#a31">[31]</a></b> Adinolfi, Daniel. “<a href="https://github.com/CVEProject/docs/blob/cna-documents/cna/CNA%20Rules/CNA%20Rules%20Development/CNA%20Rules%20v2.0week8.docx">DRAFT Common Vulnerabilities and Exposures (CVE) Numbering Authority (CNA) Rules.</a>” GitHub, 5 Oct. 2017.

<b name="f32"><a href="#a32">[32]</a></b> Evans, Jonathan. “<a href="https://cve.mitre.org/data/board/archives/2016-01/msg00016.html">RE: Updating the Products and Sources List.</a>” CVE Editorial Board Mailing List, 8 Jan. 2016.

<b name="f33"><a href="#a33">[33]</a></b> Martin, Brian. “<a href="https://cve.mitre.org/data/board/archives/2017-12/msg00004.html">Re: An Interesting Data Point.</a>” CVE Editorial Board Mailing List, 4 Dec. 2017.

<b name="f34"><a href="#a34">[34]</a></b> Franklin, Joshua, et al. “<a href="http://nvlpubs.nist.gov/nistpubs/ir/2014/NIST.IR.7946.pdf">NISTIR 7946: CVSS Implementation Guidance.</a>” National Institute of Standards and Technology, U.S. Department of Commerce.

<b name="f35"><a href="#a35">[35]</a></b> “<a href="https://nvd.nist.gov/general/faq">FAQ.</a>” National Vulnerability Database, NIST.

<b name="f36"><a href="#a36">[36]</a></b> “CVE Board Meeting Summary - 13 December 2017.” CVE Editorial Board Mailing List, 22 Dec. 2017

<b name="f37"><a href="#a37">[37]</a></b><a href="https://cve.mitre.org/about/faqs.html#cve_entry_references">Frequently Asked Questions.</a> MITRE Corporation, 2 Nov. 2017.

<b name="f38"><a href="#a38">[38]</a></b> Martin, Brian. “<a href="https://blog.osvdb.org/2016/12/19/dont_think_it_means_what_you_think_it_means/">I Do Not Think It Means What You Think It Means….</a>” OSVDB, 18 Dec. 2016.

<b name="f39"><a href="#a39">[39]</a></b> Leonov, Alexander. “<a href="https://avleonov.com/2016/11/01/forever-reserved-cves/">Forever ‘Reserved’ CVEs.</a>” Information Security Automation Blog, 2 Nov. 2016.

<b name="f40"><a href="#a40">[40]</a></b> Seifried, Kurt. “<a href="http://seclists.org/oss-sec/2016/q1/560">Distributed Weakness Filing (DWF) System.</a>” oss-sec Mailing List Archives, 7 Mar. 2016.

<b name="f41"><a href="#a41">[41]</a></b> Seifried, Kurt. “<a href="https://cve.mitre.org/data/board/archives/2017-10/msg00048.html">Article on NVD and CNNVD.</a>” CVE Editorial Board Mailing List, 19 Oct. 2017.

<b name="f42"><a href="#a42">[42]</a></b> “<a href="https://github.com/distributedweaknessfiling/cvelist">Pilot Program for CVE Submission through GitHub.</a>” GitHub, Distributed Weakness Filing.

<b name="f43"><a href="#a43">[43]</a></b> Seifried, Kurt. “<a href="https://docs.google.com/spreadsheets/d/1Jq_OpPxS5q8dLYdoWjKmklQG2AH8d9vl_2oKp-eGwA0">CVE Request Form for PUBLIC Issues in OpenSource Software v4.1 (Responses).</a>” Google Sheets.

<b name="f44"><a href="#a44">[44]</a></b> "<a href="https://github.com/CVEProject/automation-working-group">Automation Working Group.</a>" GitHub, CVEProject.

<b name="f45"><a href="#a45">[45]</a></b> “<a href="https://cve.mitre.org/data/board/archives/2017-12/msg00025.html">CVE Board Meeting Summary - 29 November 2017.</a>” CVE Editorial Board Mailing List, 12 Dec. 2017.

<b name="f46"><a href="#a46">[46]</a></b>  "<a href="https://github.com/CVEProject/cvelist/commits/master">cvelist.</a>" GitHub, CVEProject.

<b name="f47"><a href="#a47">[47]</a></b> Martin, Brian. “<a href="https://cve.mitre.org/data/board/archives/2017-12/msg00002.html">Re: An Interesting Data Point.</a>” CVE Editorial Board Mailing List, 5 Dec. 2017.

<b name="f48"><a href="#a48">[48]</a></b>  Householder, Allen. “<a href="https://insights.sei.cmu.edu/cert/2016/03/vulnerability-ids-fast-and-slow.html">Vulnerability IDs, Fast and Slow.</a>” CERT/CC Blog, Software Engineering Institute, Carnegie Mellon University, 11 Mar. 2016.

<b name="f49"><a href="#a49">[49]</a></b> "<a href="https://cve.mitre.org/about/faqs.html#update_existing_information_in_cve_entry">Frequently Asked Questions.</a>" MITRE Corporation, 2 Nov. 2017.

<b name="f50"><a href="#a50">[50]</a></b> “<a href="https://nvd.nist.gov/general/faq#eb94e293-d931-4d5b-b9f6-3812ea7fddd7">FAQ.</a>” National Vulnerability Database, NIST.

<b name="f51"><a href="#a51">[51]</a></b> "<a href="https://cve.mitre.org/about/faqs.html#disputed_signify_in_cve_entry">Frequently Asked Questions.</a>" MITRE Corporation, 2 Nov. 2017.

<b name="f52"><a href="#a52">[52]</a></b> Manion, Art. “<a href="https://cve.mitre.org/data/board/archives/2017-12/msg00029.html">Re: Convergence vs. Multiple Data Entries.</a>” CVE Editorial Board Mailing List, 13 Dec. 2017.

<b name="f53"><a href="#a53">[53]</a></b> “November 1 CVE Board Meeting Summary.” CVE Editorial Board Mailing List, 13 Nov. 2017.

<b name="f54"><a href="#a54">[54]</a></b> Seifried, Kurt. “<a href="https://cve.mitre.org/data/board/archives/2017-10/msg00015.html">CVEs with No REF URL (or a REF URL That Is Self Referential).</a>” CVE Editorial Board Mailing List, 4 Oct. 2017.

<b name="f55"><a href="#a55">[55]</a></b> Seifried, Kurt. “<a href="https://cve.mitre.org/data/board/archives/2017-05/msg00018.html">Re: Notice of Pilot Activity in CVE Auto WG.<a/>” CVE Editorial Board Mailing List, 9 May 2017.

<b name="f56"><a href="#a56">[56]</a></b> Householder, Allen. “<a href="https://insights.sei.cmu.edu/cert/2016/03/vulnerability-ids-fast-and-slow.html">Vulnerability IDs, Fast and Slow.</a>” CERT/CC Blog, Software Engineering Institute, Carnegie Mellon University, 11 Mar. 2016.

<b name="f57"><a href="#a57">[57]</a></b> "<a href="https://spdx.org/spdx-specification-21-web-version">SPDX Specification 2.1.</a>" SPDX Workgroup, a Linux Foundation Project.

<b name="f58"><a href="#a58">[58]</a></b> “<a href="http://github.com/theupdateframework/specification/blob/master/tuf-spec.md">The Update Framework Specification Version 1.0 (Draft).</a>” GitHub, 11 Oct. 2017

<b name="f59"><a href="#a59">[59]</a></b> “<a href="https://github.com/FIRSTdotorg/vrdx-sig-vxref-wip/tree/master/vxref">FIRST/vrdx-sig-vxref-wip.</a>” GitHub, FIRST.org.
