# Jenkins Execution Log

## Build Information
- **Job Name:** `MBP_Github_Polaris_Detailed_Workflow/main`
- **Build Number:** #2
- **Build Status:** 🟢 **SUCCESS**
- **Duration:** 6 min 22 sec and counting
- **Timestamp:** 2025-11-13 13:47:28 UTC

---

## Console Output

```
Branch indexing
Connecting to https://api.github.com using madhusud@blackduck.com/****** (Github_Username_PAT)
Obtained nodejs-npm/Jenkinsfile from 0ccd1a0edec3703eaacff39616ccb574f0e694d7
Loading library blackduck-logs-publisher@main
Attempting to resolve main from remote references...
 > git --version # timeout=10
 > git --version # 'git version 2.39.5 (Apple Git-154)'
using GIT_ASKPASS to set credentials Github_Username_PAT
 > git ls-remote -h -- https://github.com/integrations-garage/blackduck-logs-publisher # timeout=10
Found match: refs/heads/main revision e969196a63b1be83b84541b022f7aa52928bd5e5
The recommended git tool is: NONE
using credential Github_Username_PAT
 > git rev-parse --resolve-git-dir /Users/madhusud/.jenkins/workspace/b_Polaris_Detailed_Workflow_main@libs/a0dda568bac7bbb4a171f59ba3f2660c21c69edc6356524e9ae8bb4500c12bbb/.git # timeout=10
Fetching changes from the remote Git repository
 > git config remote.origin.url https://github.com/integrations-garage/blackduck-logs-publisher # timeout=10
Fetching without tags
Fetching upstream changes from https://github.com/integrations-garage/blackduck-logs-publisher
 > git --version # timeout=10
 > git --version # 'git version 2.39.5 (Apple Git-154)'
using GIT_ASKPASS to set credentials Github_Username_PAT
 > git fetch --no-tags --force --progress -- https://github.com/integrations-garage/blackduck-logs-publisher +refs/heads/*:refs/remotes/origin/* # timeout=10
Checking out Revision e969196a63b1be83b84541b022f7aa52928bd5e5 (main)
 > git config core.sparsecheckout # timeout=10
 > git checkout -f e969196a63b1be83b84541b022f7aa52928bd5e5 # timeout=10
Commit message: "Phase 3 - 2"
 > git rev-list --no-walk e969196a63b1be83b84541b022f7aa52928bd5e5 # timeout=10
[Pipeline] Start of Pipeline
[Pipeline] node
Running on mac-sh in /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main
[Pipeline] {
[Pipeline] stage
[Pipeline] { (Declarative: Checkout SCM)
[Pipeline] checkout
The recommended git tool is: NONE
using credential Github_Username_PAT
Fetching changes from the remote Git repository
Fetching without tags
 > git rev-parse --resolve-git-dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/.git # timeout=10
 > git config remote.origin.url https://github.com/polaris-jenkins-samples/detailed-example.git # timeout=10
Fetching upstream changes from https://github.com/polaris-jenkins-samples/detailed-example.git
 > git --version # timeout=10
 > git --version # 'git version 2.39.5 (Apple Git-154)'
using GIT_ASKPASS to set credentials Github_Username_PAT
 > git fetch --no-tags --force --progress -- https://github.com/polaris-jenkins-samples/detailed-example.git +refs/heads/main:refs/remotes/origin/main # timeout=10
Checking out Revision 0ccd1a0edec3703eaacff39616ccb574f0e694d7 (main)
Commit message: "Polaris Detailed Workflow"
First time build. Skipping changelog.
 > git config core.sparsecheckout # timeout=10
 > git checkout -f 0ccd1a0edec3703eaacff39616ccb574f0e694d7 # timeout=10
 > git rev-list --no-walk 91f9657ca2379476de1cee53c2fe6ada9d703715 # timeout=10
[Pipeline] }
[Pipeline] // stage
[Pipeline] withEnv
[Pipeline] {
[Pipeline] stage
[Pipeline] { (Build)
[Pipeline] script
[Pipeline] {
[Pipeline] echo
JOB_NAME: MBP_Github_Polaris_Detailed_Workflow/main
[Pipeline] dir
Running in /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm
[Pipeline] {
[Pipeline] sh
+ node --version
v22.16.0
[Pipeline] sh
+ npm --version
10.9.2
[Pipeline] sh
+ npm install
npm warn deprecated fsevents@1.2.9: fsevents 1 will break on node v14+ and could be using insecure binaries. Upgrade to fsevents 2.
npm warn deprecated set-value@2.0.0: Critical bug fixed in v3.0.1, please upgrade to the latest version.
npm warn deprecated mixin-deep@1.3.1: Critical bug fixed in v2.0.1, please upgrade to the latest version.
npm warn deprecated ini@1.3.5: Please update to ini >=1.3.6 to avoid a prototype pollution issue
npm warn deprecated set-value@0.4.3: Critical bug fixed in v3.0.1, please upgrade to the latest version.
npm warn deprecated path-is-absolute@2.0.0: This package is no longer relevant as Node.js 0.12 is unmaintained.
npm warn deprecated urix@0.1.0: Please see https://github.com/lydell/urix#deprecated
npm warn deprecated har-validator@5.1.3: this library is no longer supported
npm warn deprecated to-iso-string@0.0.2: to-iso-string has been deprecated, use @segment/to-iso-string instead.
npm warn deprecated cryptiles@2.0.5: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated resolve-url@0.2.1: https://github.com/lydell/resolve-url#deprecated
npm warn deprecated bcrypt-nodejs@0.0.3: bcrypt-nodejs is no longer actively maintained. Please use bcrypt or bcryptjs. See https://github.com/kelektiv/node.bcrypt.js/wiki/bcrypt-vs-brypt.js to learn more about these two options
npm warn deprecated cryptiles@0.2.2: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated source-map-url@0.4.0: See https://github.com/lydell/source-map-url#deprecated
npm warn deprecated boom@0.4.2: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated debug@3.2.6: Debug versions >=3.2.0 <3.2.7 || >=4 <4.3.1 have a low-severity ReDos regression when used in a Node.js environment. It is recommended you upgrade to 3.2.7 or 4.3.1. (https://github.com/visionmedia/debug/issues/797)
npm warn deprecated debug@3.2.6: Debug versions >=3.2.0 <3.2.7 || >=4 <4.3.1 have a low-severity ReDos regression when used in a Node.js environment. It is recommended you upgrade to 3.2.7 or 4.3.1. (https://github.com/visionmedia/debug/issues/797)
npm warn deprecated debug@3.2.6: Debug versions >=3.2.0 <3.2.7 || >=4 <4.3.1 have a low-severity ReDos regression when used in a Node.js environment. It is recommended you upgrade to 3.2.7 or 4.3.1. (https://github.com/visionmedia/debug/issues/797)
npm warn deprecated debug@3.2.6: Debug versions >=3.2.0 <3.2.7 || >=4 <4.3.1 have a low-severity ReDos regression when used in a Node.js environment. It is recommended you upgrade to 3.2.7 or 4.3.1. (https://github.com/visionmedia/debug/issues/797)
npm warn deprecated boom@2.10.1: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated chokidar@2.1.6: Chokidar 2 does not receive security updates since 2019. Upgrade to chokidar 3 with 15x fewer dependencies
npm warn deprecated sntp@0.2.4: This module moved to @hapi/sntp. Please make sure to switch over as this distribution is no longer supported and may contain bugs and critical security issues.
npm warn deprecated minimatch@0.3.0: Please update to minimatch 3.0.2 or higher to avoid a RegExp DoS issue
npm warn deprecated chokidar@2.1.8: Chokidar 2 does not receive security updates since 2019. Upgrade to chokidar 3 with 15x fewer dependencies
npm warn deprecated sntp@1.0.9: This module moved to @hapi/sntp. Please make sure to switch over as this distribution is no longer supported and may contain bugs and critical security issues.
npm warn deprecated querystring@0.2.0: The querystring API is considered Legacy. new code should use the URLSearchParams API instead.
npm warn deprecated request@2.36.0: request has been deprecated, see https://github.com/request/request/issues/3142
npm warn deprecated mkdirp@0.3.0: Legacy versions of mkdirp are no longer supported. Please update to mkdirp 1.x. (Note that the API surface has changed to use Promises in 1.x.)
npm warn deprecated tough-cookie@2.2.2: ReDoS vulnerability parsing Set-Cookie https://nodesecurity.io/advisories/130
npm warn deprecated hoek@0.9.1: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated node-uuid@1.4.8: Use uuid module instead
npm warn deprecated node-uuid@1.4.8: Use uuid module instead
npm warn deprecated uuid@3.3.2: Please upgrade  to version 7 or higher.  Older versions may use Math.random() in certain circumstances, which is known to be problematic.  See https://v8.dev/blog/math-random for details.
npm warn deprecated source-map-resolve@0.5.2: See https://github.com/lydell/source-map-resolve#deprecated
npm warn deprecated har-validator@2.0.6: this library is no longer supported
npm warn deprecated mkdirp@0.5.1: Legacy versions of mkdirp are no longer supported. Please update to mkdirp 1.x. (Note that the API surface has changed to use Promises in 1.x.)
npm warn deprecated hoek@2.16.3: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated request@2.79.0: request has been deprecated, see https://github.com/request/request/issues/3142
npm warn deprecated request@2.88.0: request has been deprecated, see https://github.com/request/request/issues/3142
npm warn deprecated request@2.67.0: request has been deprecated, see https://github.com/request/request/issues/3142
npm warn deprecated readdir-scoped-modules@1.0.2: This functionality has been moved to @npmcli/fs
npm warn deprecated hawk@1.0.0: This module moved to @hapi/hawk. Please make sure to switch over as this distribution is no longer supported and may contain bugs and critical security issues.
npm warn deprecated hawk@3.1.3: This module moved to @hapi/hawk. Please make sure to switch over as this distribution is no longer supported and may contain bugs and critical security issues.
npm warn deprecated jade@0.26.3: Jade has been renamed to pug, please install the latest version of pug instead of jade
npm warn deprecated swig@1.4.2: This package is no longer maintained
npm warn deprecated bson@1.0.9: Fixed a critical issue with BSON serialization documented in CVE-2019-2391, see https://bit.ly/2KcpXdo for more details
npm warn deprecated nodeunit@0.9.5: you are strongly encouraged to use other testing options

added 962 packages, and audited 1412 packages in 23s

32 packages are looking for funding
  run `npm fund` for details

136 vulnerabilities (9 low, 35 moderate, 57 high, 35 critical)

To address issues that do not require attention, run:
  npm audit fix

To address all issues possible (including breaking changes), run:
  npm audit fix --force

Some issues need review, and may require choosing
a different dependency.

Run `npm audit` for details.
[Pipeline] }
[Pipeline] // dir
[Pipeline] }
[Pipeline] // script
[Pipeline] }
[Pipeline] // stage
[Pipeline] stage
[Pipeline] { (polaris-detailed-workflow)
[Pipeline] script
[Pipeline] {
[Pipeline] dir
Running in /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm
[Pipeline] {
[Pipeline] security_scan
**************************** START EXECUTION OF BLACK DUCK SECURITY SCAN ****************************
[Security Scan] INFO: Jenkins Job name: MBP_Github_Polaris_Detailed_Workflow
-------------------------------- Connection to node --------------------------------
[Security Scan] INFO: Jenkins job is running on agent node remotely
-------------------------- Parameter Validation Initiated --------------------------
[Security Scan] INFO:  --- product = [POLARIS]
[Security Scan] INFO: Parameters for polaris:
[Security Scan] INFO:  --- coverity_clean_command = npm cache clean --force
[Security Scan] INFO:  --- detect_search_depth = 3
[Security Scan] INFO:  --- polaris_reports_sarif_groupSCAIssues = true
[Security Scan] INFO:  --- polaris_reports_sarif_create = true
[Security Scan] INFO:  --- polaris_test_sca_location = hybrid
[Security Scan] INFO:  --- polaris_prComment_severities = CRITICAL,HIGH
[Security Scan] INFO:  --- polaris_reports_sarif_issue_types = SAST, SCA
[Security Scan] INFO:  --- polaris_waitForScan = true
[Security Scan] INFO:  --- polaris_server_url = https://poc.polaris.blackduck.com
[Security Scan] INFO:  --- polaris_assessment_types = SAST,SCA
[Security Scan] INFO:  --- polaris_access_token = ******************************************************************************
[Security Scan] INFO:  --- polaris_prComment_enabled = true
[Security Scan] INFO:  --- detect_args = --detect.diagnostic=true
[Security Scan] INFO:  --- polaris_test_sast_location = hybrid
[Security Scan] INFO:  --- coverity_build_command = npm install
[Security Scan] INFO:  --- polaris_reports_sarif_severities = CRITICAL,HIGH
------------------------------------------------------------------------------------
[Security Scan] INFO: Parameters for additional configuration:
[Security Scan] INFO:  --- network_airgap = false
[Security Scan] INFO: Polaris parameters are validated successfully
[Security Scan] INFO: Bridge download parameters are validated successfully
[Security Scan] INFO: Bridge download is not required. Found installed in: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm
------------------------------------------------------------------------------------
[Security Scan] INFO: Bridge CLI version is - 3.9.2
[Security Scan] INFO: Jenkins Job name: MBP_Github_Polaris_Detailed_Workflow
[Security Scan] INFO: Polaris Application Name: detailed-example
[Security Scan] INFO: Polaris Project Name: detailed-example
[Security Scan] INFO: Polaris Branch Name: main
[Security Scan] INFO: Polaris PR Comment is ignored for non pull request scan
[Security Scan] INFO: Jenkins Job name: MBP_Github_Polaris_Detailed_Workflow
[Security Scan] INFO: Executable command line arguments: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm/bridge-cli --stage polaris --input /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/polaris_input8053108785247146626.json --out .bridge/output/scan_info_out.json

******************************* START EXECUTION OF BRIDGE CLI *******************************
2025-11-13 13:41:42.9862 IST [Bridge CLI] INFO: Using cache directory: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm
2025-11-13 13:41:42.9972 IST [Bridge CLI] INFO: Found version "3.0.371" in registry for workflow "polaris", trying to load it from local cache
2025-11-13 13:41:44.2938 IST [Bridge CLI] INFO: Input Resources:
2025-11-13 13:41:44.2939 IST [Bridge CLI] INFO: resource = value [source]
2025-11-13 13:41:44.2939 IST [Bridge CLI] INFO: ------------------------------------------------------------
2025-11-13 13:41:44.2939 IST [Bridge CLI] INFO: coverity.build.command = npm install [polaris_input8053108785247146626.json]
2025-11-13 13:41:44.2939 IST [Bridge CLI] INFO: coverity.clean.command = npm cache clean --force [polaris_input8053108785247146626.json]
2025-11-13 13:41:44.2939 IST [Bridge CLI] INFO: detect.args = --detect.diagnostic=true [polaris_input8053108785247146626.json]
2025-11-13 13:41:44.2939 IST [Bridge CLI] INFO: detect.search.depth = 3 [polaris_input8053108785247146626.json]
2025-11-13 13:41:44.2939 IST [Bridge CLI] INFO: network.airgap = false [polaris_input8053108785247146626.json]
2025-11-13 13:41:44.2940 IST [Bridge CLI] INFO: polaris.accesstoken = ***************************************** [polaris_input8053108785247146626.json]
2025-11-13 13:41:44.2940 IST [Bridge CLI] INFO: polaris.application.name = detailed-example [polaris_input8053108785247146626.json]
2025-11-13 13:41:44.2940 IST [Bridge CLI] INFO: polaris.assessment.types = [SAST SCA] [polaris_input8053108785247146626.json]
2025-11-13 13:41:44.2940 IST [Bridge CLI] INFO: polaris.branch.name = main [polaris_input8053108785247146626.json]
2025-11-13 13:41:44.2940 IST [Bridge CLI] INFO: polaris.project.name = detailed-example [polaris_input8053108785247146626.json]
2025-11-13 13:41:44.2940 IST [Bridge CLI] INFO: polaris.reports.sarif.create = true [polaris_input8053108785247146626.json]
2025-11-13 13:41:44.2940 IST [Bridge CLI] INFO: polaris.reports.sarif.file.path = .blackduck/integrations/polaris/sarif/report.sarif.json [polaris_input8053108785247146626.json]
2025-11-13 13:41:44.2940 IST [Bridge CLI] INFO: polaris.reports.sarif.groupSCAIssues = true [polaris_input8053108785247146626.json]
2025-11-13 13:41:44.2940 IST [Bridge CLI] INFO: polaris.reports.sarif.issue.types = [SAST SCA] [polaris_input8053108785247146626.json]
2025-11-13 13:41:44.2940 IST [Bridge CLI] INFO: polaris.reports.sarif.severities = [CRITICAL HIGH] [polaris_input8053108785247146626.json]
2025-11-13 13:41:44.2940 IST [Bridge CLI] INFO: polaris.serverUrl = https://poc.polaris.blackduck.com [polaris_input8053108785247146626.json]
2025-11-13 13:41:44.2940 IST [Bridge CLI] INFO: polaris.test.sast.location = hybrid [polaris_input8053108785247146626.json]
2025-11-13 13:41:44.2940 IST [Bridge CLI] INFO: polaris.test.sca.location = hybrid [polaris_input8053108785247146626.json]
2025-11-13 13:41:44.2941 IST [Bridge CLI] INFO: polaris.waitForScan = true [polaris_input8053108785247146626.json]
2025-11-13 13:41:44.2941 IST [Bridge CLI] INFO: ------------------------------------------------------------
2025-11-13 13:41:44.2941 IST [Bridge CLI] INFO: Starting adapters for stage polaris
2025-11-13 13:41:44.2957 IST [Bridge CLI] INFO: Starting Adapter: Polaris Status Provider
2025-11-13 13:41:44.2958 IST [Bridge CLI] INFO: Starting Adapter: Polaris Initializer
2025-11-13 13:41:44.2958 IST [Bridge CLI] INFO: Starting Adapter: Polaris SCM Discovery
2025-11-13 13:41:44.2958 IST [Bridge CLI] INFO: Starting Adapter: Polaris Controller
2025-11-13 13:41:44.3711 IST [Polaris SCM Discovery] INFO: Adapter finished
2025-11-13 13:41:44.3763 IST [Bridge CLI] INFO: Starting Adapter: Set Polaris Assessment Mode to CI
2025-11-13 13:41:44.3764 IST [Set Polaris Assessment Mode to CI] INFO: Provided value for resource 'polaris.assessment.mode'
2025-11-13 13:41:44.3765 IST [Set Polaris Assessment Mode to CI] INFO: Adapter finished
2025-11-13 13:41:44.3805 IST [Bridge CLI] INFO: Starting Adapter: Create Polaris Project & Branch By Default
2025-11-13 13:41:44.3807 IST [Create Polaris Project & Branch By Default] INFO: Provided value for resource 'polaris.onboarding'
2025-11-13 13:41:44.3807 IST [Create Polaris Project & Branch By Default] INFO: Adapter finished
2025-11-13 13:41:47.2513 IST [Polaris Initializer] INFO: Successfully created test for "SAST(sastFull)" assessment. The short test ID is "THMXN70"
2025-11-13 13:41:47.2513 IST [Polaris Initializer] INFO: Successfully created test for "SCA(scaPackage)" assessment. The short test ID is "V3W07JK"
2025-11-13 13:41:47.2763 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.id'
2025-11-13 13:41:47.2768 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.id'
2025-11-13 13:41:47.2772 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.shortId'
2025-11-13 13:41:47.2774 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.shortId'
2025-11-13 13:41:47.2776 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.streamId'
2025-11-13 13:41:47.2777 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.project.id'
2025-11-13 13:41:47.2779 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.branch.id'
2025-11-13 13:41:47.2780 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.portfolioid'
2025-11-13 13:41:47.2782 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.tenant.id'
2025-11-13 13:41:47.2783 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.application.id'
2025-11-13 13:41:47.2786 IST [Polaris Initializer] INFO: Adapter finished
2025-11-13 13:41:47.2926 IST [Bridge CLI] INFO: Starting Adapter: Check pull request
2025-11-13 13:41:47.3356 IST [Check pull request] INFO: Provided value for resource 'environment.scan.pull'
2025-11-13 13:41:47.3359 IST [Check pull request] INFO: Adapter finished
2025-11-13 13:41:47.3882 IST [Polaris Controller] INFO: Running for "sast" assessment with scan type "sastFull"
2025-11-13 13:41:47.3885 IST [Polaris Controller] INFO: fetching recommended "coverity" tool info...
2025-11-13 13:41:48.2421 IST [Polaris Controller] INFO: checking "coverity" tool installation inside bridge home directory: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0
2025-11-13 13:41:48.2423 IST [Polaris Controller] INFO: Checking tool version for "cov_thin_client" in "/Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0"
2025-11-13 13:41:48.2424 IST [Polaris Controller] INFO: Running command:/Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/coverity --version
2025-11-13 13:41:48.3262 IST [Polaris Controller] INFO: Got tool version for "cov_thin_client": 2025.9.0
2025-11-13 13:41:48.6325 IST [Polaris Controller] INFO: "coverity" tool is already installed...
2025-11-13 13:41:48.6327 IST [Polaris Controller] INFO: fetching recommended "Sigma" tool info...
2025-11-13 13:41:48.9101 IST [Polaris Controller] INFO: checking "Sigma" tool installation inside bridge home directory: /Users/madhusud/.blackduck/bridge/tools/sigma/2025.10.0
2025-11-13 13:41:48.9102 IST [Polaris Controller] INFO: Checking tool version for "sigma" in "/Users/madhusud/.blackduck/bridge/tools/sigma/2025.10.0"
2025-11-13 13:41:48.9106 IST [Polaris Controller] INFO: Running command:/Users/madhusud/.blackduck/bridge/tools/sigma/2025.10.0/sigma --version
2025-11-13 13:41:49.0128 IST [Polaris Controller] INFO: Got tool version for "sigma": 2025.10.0
2025-11-13 13:41:49.3128 IST [Polaris Controller] INFO: "Sigma" tool is already installed...
2025-11-13 13:41:49.3129 IST [Polaris Controller] INFO: Running for "sca" assessment with scan type "scaPackage"
2025-11-13 13:41:49.3129 IST [Polaris Controller] INFO: fetching recommended "detect" tool info...
2025-11-13 13:41:49.6002 IST [Polaris Controller] INFO: checking "detect" tool installation inside bridge home directory: /Users/madhusud/.blackduck/bridge/tools/blackduck-detect/10.4.0
2025-11-13 13:41:49.6003 IST [Polaris Controller] INFO: Running command:/Library/Java/JavaVirtualMachines/jdk-21.jdk/Contents/Home/bin/java -version
2025-11-13 13:41:49.6836 IST [Polaris Controller] INFO: Checking tool version for "detect" in "/Users/madhusud/.blackduck/bridge/tools/blackduck-detect/10.4.0"
2025-11-13 13:41:49.6869 IST [Polaris Controller] INFO: Got tool version for "detect": 10.4.0
2025-11-13 13:41:49.9670 IST [Polaris Controller] INFO: "detect" tool is already installed...
2025-11-13 13:41:49.9963 IST [Polaris Controller] INFO: Provided value for resource 'coverity.id'
2025-11-13 13:41:49.9966 IST [Polaris Controller] INFO: Provided value for resource 'sigma.id'
2025-11-13 13:41:49.9968 IST [Polaris Controller] INFO: Provided value for resource 'detect.id'
2025-11-13 13:41:49.9970 IST [Bridge CLI] INFO: Starting adapters for stage polaris-sast
2025-11-13 13:41:49.9970 IST [Bridge CLI] INFO: Starting adapters for stage polaris-sca-package
2025-11-13 13:41:49.9970 IST [Bridge CLI] INFO: Starting adapters for stage polaris-artifacts-uploader
2025-11-13 13:41:49.9970 IST [Bridge CLI] INFO: Starting adapters for stage polaris-post-processing
2025-11-13 13:41:49.9970 IST [Bridge CLI] INFO: Starting adapters for stage polaris-reports-sarif
2025-11-13 13:41:50.0017 IST [Bridge CLI] INFO: Starting Adapter: Polaris SCA Package Manager Scan
2025-11-13 13:41:50.0030 IST [Bridge CLI] INFO: Starting Adapter: Polaris Coverity Capture
2025-11-13 13:41:50.0034 IST [Bridge CLI] INFO: Starting Adapter: Polaris Artifacts Uploader
2025-11-13 13:41:50.0035 IST [Bridge CLI] INFO: Starting Adapter: Polaris Policy Checker
2025-11-13 13:41:50.0035 IST [Bridge CLI] INFO: Starting Adapter: Polaris Issues Fetcher
2025-11-13 13:41:50.0035 IST [Bridge CLI] INFO: Starting Adapter: Polaris Waiter
2025-11-13 13:41:50.0036 IST [Bridge CLI] INFO: Starting Adapter: Polaris SARIF Issues Fetcher
2025-11-13 13:41:50.0036 IST [Polaris Controller] INFO: Adapter finished
2025-11-13 13:41:50.0557 IST [Bridge CLI] INFO: Starting Adapter: Default Adapter for execution path
2025-11-13 13:41:50.0561 IST [Default Adapter for execution path] INFO: Provided value for resource 'coverity.execution.path'
2025-11-13 13:41:50.0562 IST [Default Adapter for execution path] INFO: Adapter finished
2025-11-13 13:41:50.0756 IST [Bridge CLI] INFO: Starting Adapter: Default Adapter for execution path
2025-11-13 13:41:50.0757 IST [Default Adapter for execution path] INFO: Provided value for resource 'sigma.execution.path'
2025-11-13 13:41:50.0758 IST [Default Adapter for execution path] INFO: Adapter finished
2025-11-13 13:41:50.1368 IST [Polaris Coverity Capture] INFO: Identified workflow: Polaris
2025-11-13 13:41:50.1375 IST [Polaris Coverity Capture] INFO: command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/coverity capture --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir -o capture.build.clean-command=npm cache clean --force -o analyze.location=connect -- npm install
2025-11-13 13:41:50.2286 IST [Polaris Coverity Capture] INFO: coverity 2025.9.0 covcli-2025.9-push-12
2025-11-13 13:41:50.2287 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CACHE_API_TOKEN_FILE=/var/folders/wm/gkd75sk54h57yqd0_j95gp2r0000gn/T/polaris_coverity_cache2274679289/.authKey
2025-11-13 13:41:50.2287 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CACHE_KEY=ceac6937-e678-4b1e-9838-f1a4cdc36d87
2025-11-13 13:41:50.2287 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CACHE_URL=https://poc.polaris.blackduck.com/api/cache
2025-11-13 13:41:50.2287 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CLI_CAPTURE_ZIP_ARCHIVE=/Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_coverity_capture/idir.zip
2025-11-13 13:41:50.2287 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CLI_POLARIS_CLIENT=true
2025-11-13 13:41:50.2300 IST [Polaris Coverity Capture] INFO: Detected that stdout is not connected to a terminal.  Defaulting ticker mode to 'none'.
2025-11-13 13:41:50.2300 IST [Polaris Coverity Capture] INFO: If this is not correct, explicitly set the ticker mode to the desired value using the '--ticker-mode' option.
2025-11-13 13:41:50.2309 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir create
2025-11-13 13:41:50.2821 IST [Polaris Coverity Capture] INFO: Using lightweight capture with thin client.
2025-11-13 13:41:50.2823 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-internal-manage-cache check
2025-11-13 13:41:51.1426 IST [Polaris Coverity Capture] INFO: Caching is enabled.
2025-11-13 13:41:51.1464 IST [Polaris Coverity Capture] INFO: Telemetry is enabled
2025-11-13 13:41:51.6457 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir list-capture-diagnostics
2025-11-13 13:41:51.6592 IST [Polaris Coverity Capture] INFO: Executing action no-op: nothing to do for initialization
2025-11-13 13:41:52.1020 IST [Polaris Coverity Capture] INFO: Executing action Delete compiler configurations for intermediate directory '/Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir'
2025-11-13 13:41:52.1021 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler gcc --comptype clangcc --template
2025-11-13 13:41:52.3855 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler cc --comptype gcc --template
2025-11-13 13:41:52.6154 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler c++ --comptype g++ --template
2025-11-13 13:41:52.8540 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler clang --comptype clangcc --template
2025-11-13 13:41:53.0929 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler java --comptype java --template
2025-11-13 13:41:53.3275 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler go --comptype go --template
2025-11-13 13:41:53.5820 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler ccache --comptype prefix --template
2025-11-13 13:41:53.8195 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler kotlinc --comptype kotlinc --template
2025-11-13 13:41:54.0550 IST [Polaris Coverity Capture] WARNING: Template config template-java-config-0 already exists for java and will be reused. 
2025-11-13 13:41:54.0551 IST [Polaris Coverity Capture] WARNING: Template config template-apt-config-0 already exists for apt and will be reused. 
2025-11-13 13:41:54.0551 IST [Polaris Coverity Capture] WARNING: Template config template-javaw-config-0 already exists for javaw and will be reused. 
2025-11-13 13:41:54.0731 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --dart
2025-11-13 13:41:54.3026 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --javascript
2025-11-13 13:41:54.5358 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --php
2025-11-13 13:41:54.7712 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --python
2025-11-13 13:41:55.0165 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --ruby
2025-11-13 13:41:55.2463 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --comptype capture-config-files --file-regex $capture-config-files$ --template
2025-11-13 13:41:55.2640 IST [Polaris Coverity Capture] WARNING: Configuration already exists for file regex $capture-config-files$
2025-11-13 13:41:55.2641 IST [Polaris Coverity Capture] INFO:           and it will not be updated.
2025-11-13 13:41:55.7103 IST [Polaris Coverity Capture] INFO: Executing action no-op: no compilers need to be unconfigured
2025-11-13 13:41:56.1312 IST [Polaris Coverity Capture] INFO: Executing action no-op: compiler configurations loaded
2025-11-13 13:41:56.6001 IST [Polaris Coverity Capture] INFO: Executing action Execute clean command: sh -c npm cache clean --force
2025-11-13 13:41:56.7485 IST [Polaris Coverity Capture] INFO: npm warn using --force Recommended protections disabled.
2025-11-13 13:41:57.9558 IST [Polaris Coverity Capture] INFO: Executing action Invoke build capture: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-build --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --append-log --no-security-da --record-with-source --no-xrefs --enable-scan-transparency-data --bytecode-caching --force npm install
2025-11-13 13:41:57.9919 IST [Polaris Coverity Capture] INFO: Coverity Build Capture (64-bit) version 2025.9.0 on Darwin 24.6.0 arm64
2025-11-13 13:41:57.9919 IST [Polaris Coverity Capture] INFO: Internal version numbers: 477d3c5ddd p-2025.9-push-57
2025-11-13 13:41:57.9919 IST [Polaris Coverity Capture] INFO: 
2025-11-13 13:41:58.0044 IST [Polaris Coverity Capture] INFO: 
2025-11-13 13:42:55.9594 IST [Polaris Coverity Capture] INFO: npm warn deprecated urix@0.1.0: Please see https://github.com/lydell/urix#deprecated
2025-11-13 13:42:55.9778 IST [Polaris Coverity Capture] INFO: npm warn deprecated source-map-url@0.4.1: See https://github.com/lydell/source-map-url#deprecated
2025-11-13 13:42:55.9778 IST [Polaris Coverity Capture] INFO: npm warn deprecated resolve-url@0.2.1: https://github.com/lydell/resolve-url#deprecated
2025-11-13 13:42:56.6896 IST [Polaris Coverity Capture] INFO: npm warn deprecated source-map-resolve@0.5.3: See https://github.com/lydell/source-map-resolve#deprecated
2025-11-13 13:42:57.9664 IST [Polaris Coverity Capture] INFO: npm warn deprecated stable@0.1.8: Modern JS already guarantees Array#sort() is a stable sort, so this library is deprecated. See the compatibility table on MDN: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/sort#browser_compatibility
2025-11-13 13:42:58.2607 IST [Polaris Coverity Capture] INFO: npm warn deprecated try-resolve@1.0.1: Package no longer supported. Contact Support at https://www.npmjs.com/support for more info.
2025-11-13 13:42:58.3901 IST [Polaris Coverity Capture] INFO: npm warn deprecated babel-plugin-undefined-to-void@1.1.6: Package no longer supported. Contact Support at https://www.npmjs.com/support for more info.
2025-11-13 13:42:58.4964 IST [Polaris Coverity Capture] INFO: npm warn deprecated babel-plugin-remove-debugger@1.0.1: Package no longer supported. Contact Support at https://www.npmjs.com/support for more info.
2025-11-13 13:42:58.5258 IST [Polaris Coverity Capture] INFO: npm warn deprecated babel-plugin-react-constant-elements@1.0.3: Package no longer supported. Contact Support at https://www.npmjs.com/support for more info.
2025-11-13 13:42:58.5276 IST [Polaris Coverity Capture] INFO: npm warn deprecated babel-plugin-property-literals@1.0.1: Package no longer supported. Contact Support at https://www.npmjs.com/support for more info.
2025-11-13 13:42:58.5277 IST [Polaris Coverity Capture] INFO: npm warn deprecated babel-plugin-remove-console@1.0.1: Package no longer supported. Contact Support at https://www.npmjs.com/support for more info.
2025-11-13 13:42:58.5295 IST [Polaris Coverity Capture] INFO: npm warn deprecated babel-plugin-react-display-name@1.0.3: Package no longer supported. Contact Support at https://www.npmjs.com/support for more info.
2025-11-13 13:42:58.5300 IST [Polaris Coverity Capture] INFO: npm warn deprecated babel-plugin-proto-to-assign@1.0.4: Package no longer supported. Contact Support at https://www.npmjs.com/support for more info.
2025-11-13 13:42:58.5305 IST [Polaris Coverity Capture] INFO: npm warn deprecated babel-plugin-member-expression-literals@1.0.1: Package no longer supported. Contact Support at https://www.npmjs.com/support for more info.
2025-11-13 13:42:58.5409 IST [Polaris Coverity Capture] INFO: npm warn deprecated babel-plugin-jscript@1.0.4: Package no longer supported. Contact Support at https://www.npmjs.com/support for more info.
2025-11-13 13:42:58.5902 IST [Polaris Coverity Capture] INFO: npm warn deprecated babel-plugin-dead-code-elimination@1.0.2: Package no longer supported. Contact Support at https://www.npmjs.com/support for more info.
2025-11-13 13:42:58.5967 IST [Polaris Coverity Capture] INFO: npm warn deprecated babel-plugin-inline-environment-variables@1.0.1: Package no longer supported. Contact Support at https://www.npmjs.com/support for more info.
2025-11-13 13:42:58.6284 IST [Polaris Coverity Capture] INFO: npm warn deprecated babel-plugin-eval@1.0.1: Package no longer supported. Contact Support at https://www.npmjs.com/support for more info.
2025-11-13 13:42:58.6356 IST [Polaris Coverity Capture] INFO: npm warn deprecated babel-plugin-constant-folding@1.0.1: Package no longer supported. Contact Support at https://www.npmjs.com/support for more info.
2025-11-13 13:42:58.7623 IST [Polaris Coverity Capture] INFO: npm warn deprecated babel-plugin-runtime@1.0.7: Package no longer supported. Contact Support at https://www.npmjs.com/support for more info.
2025-11-13 13:42:59.7521 IST [Polaris Coverity Capture] INFO: npm warn deprecated q@0.8.12: You or someone you depend on is using Q, the JavaScript Promise library that gave JavaScript developers strong feelings about promises. They can almost certainly migrate to the native JavaScript promise now. Thank you literally everyone for joining me in this bet against the odds. Be excellent to each other.
2025-11-13 13:42:59.7521 IST [Polaris Coverity Capture] INFO: npm warn deprecated
2025-11-13 13:42:59.7521 IST [Polaris Coverity Capture] INFO: npm warn deprecated (For a CapTP with native promises, see @endo/eventual-send and @endo/captp)
2025-11-13 13:43:00.5052 IST [Polaris Coverity Capture] INFO: npm warn deprecated json3@3.3.2: Please use the native JSON object instead of JSON 3
2025-11-13 13:43:01.4559 IST [Polaris Coverity Capture] INFO: npm warn deprecated constantinople@3.0.2: Please update to at least constantinople 3.1.1
2025-11-13 13:43:01.4715 IST [Polaris Coverity Capture] INFO: npm warn deprecated transformers@2.1.0: Deprecated, use jstransformer
2025-11-13 13:43:02.4562 IST [Polaris Coverity Capture] INFO: npm warn deprecated rimraf@2.6.3: Rimraf versions prior to v4 are no longer supported
2025-11-13 13:43:02.4563 IST [Polaris Coverity Capture] INFO: npm warn deprecated inflight@1.0.6: This module is not supported, and leaks memory. Do not use it. Check out lru-cache if you want a good and tested way to coalesce async requests by a key value, which is much more comprehensive and powerful.
2025-11-13 13:43:02.5007 IST [Polaris Coverity Capture] INFO: npm warn deprecated circular-json@0.3.3: CircularJSON is in maintenance only, flatted is its successor.
2025-11-13 13:43:03.2690 IST [Polaris Coverity Capture] INFO: npm warn deprecated coffee-script@1.12.7: CoffeeScript on NPM has moved to "coffeescript" (no hyphen)
2025-11-13 13:43:03.2692 IST [Polaris Coverity Capture] INFO: npm warn deprecated glob@7.2.3: Glob versions prior to v9 are no longer supported
2025-11-13 13:43:04.0168 IST [Polaris Coverity Capture] INFO: npm warn deprecated core-js@2.6.12: core-js@<3.23.3 is no longer maintained and not recommended for usage due to the number of issues. Because of the V8 engine whims, feature detection in old core-js versions could cause a slowdown up to 100x even if nothing is polyfilled. Some versions have web compatibility issues. Please, upgrade your dependencies to the actual version of core-js.
2025-11-13 13:43:04.5447 IST [Polaris Coverity Capture] INFO: npm warn deprecated swig@1.4.2: This package is no longer maintained
2025-11-13 13:43:04.7405 IST [Polaris Coverity Capture] INFO: npm warn deprecated jade@1.11.0: Jade has been renamed to pug, please install the latest version of pug instead of jade
2025-11-13 13:43:05.2452 IST [Polaris Coverity Capture] INFO: npm warn deprecated eslint@3.19.0: This version is no longer supported. Please see https://eslint.org/version-support for other options.
2025-11-13 13:43:06.1732 IST [Polaris Coverity Capture] INFO: npm warn deprecated q@1.5.1: You or someone you depend on is using Q, the JavaScript Promise library that gave JavaScript developers strong feelings about promises. They can almost certainly migrate to the native JavaScript promise now. Thank you literally everyone for joining me in this bet against the odds. Be excellent to each other.
2025-11-13 13:43:06.1733 IST [Polaris Coverity Capture] INFO: npm warn deprecated
2025-11-13 13:43:06.1733 IST [Polaris Coverity Capture] INFO: npm warn deprecated (For a CapTP with native promises, see @endo/eventual-send and @endo/captp)
2025-11-13 13:43:06.1902 IST [Polaris Coverity Capture] INFO: npm warn deprecated glob@5.0.15: Glob versions prior to v9 are no longer supported
2025-11-13 13:43:06.4968 IST [Polaris Coverity Capture] INFO: npm warn deprecated core-js@1.2.7: core-js@<3.23.3 is no longer maintained and not recommended for usage due to the number of issues. Because of the V8 engine whims, feature detection in old core-js versions could cause a slowdown up to 100x even if nothing is polyfilled. Some versions have web compatibility issues. Please, upgrade your dependencies to the actual version of core-js.
2025-11-13 13:43:06.6086 IST [Polaris Coverity Capture] INFO: npm warn deprecated q@1.5.1: You or someone you depend on is using Q, the JavaScript Promise library that gave JavaScript developers strong feelings about promises. They can almost certainly migrate to the native JavaScript promise now. Thank you literally everyone for joining me in this bet against the odds. Be excellent to each other.
2025-11-13 13:43:06.6087 IST [Polaris Coverity Capture] INFO: npm warn deprecated
2025-11-13 13:43:06.6087 IST [Polaris Coverity Capture] INFO: npm warn deprecated (For a CapTP with native promises, see @endo/eventual-send and @endo/captp)
2025-11-13 13:43:06.9456 IST [Polaris Coverity Capture] INFO: npm warn deprecated glob@3.2.11: Glob versions prior to v9 are no longer supported
2025-11-13 13:43:06.9703 IST [Polaris Coverity Capture] INFO: npm warn deprecated minimatch@0.3.0: Please update to minimatch 3.0.2 or higher to avoid a RegExp DoS issue
2025-11-13 13:43:07.6324 IST [Polaris Coverity Capture] INFO: npm warn deprecated core-js@1.2.7: core-js@<3.23.3 is no longer maintained and not recommended for usage due to the number of issues. Because of the V8 engine whims, feature detection in old core-js versions could cause a slowdown up to 100x even if nothing is polyfilled. Some versions have web compatibility issues. Please, upgrade your dependencies to the actual version of core-js.
2025-11-13 13:43:07.6656 IST [Polaris Coverity Capture] INFO: npm warn deprecated mkdirp@0.5.1: Legacy versions of mkdirp are no longer supported. Please update to mkdirp 1.x. (Note that the API surface has changed to use Promises in 1.x.)
2025-11-13 13:43:07.7128 IST [Polaris Coverity Capture] INFO: npm warn deprecated glob@7.1.1: Glob versions prior to v9 are no longer supported
2025-11-13 13:43:07.9559 IST [Polaris Coverity Capture] INFO: npm warn deprecated mkdirp@0.3.0: Legacy versions of mkdirp are no longer supported. Please update to mkdirp 1.x. (Note that the API surface has changed to use Promises in 1.x.)
2025-11-13 13:43:08.4260 IST [Polaris Coverity Capture] INFO: npm warn deprecated fsevents@1.2.13: Upgrade to fsevents v2 to mitigate potential security issues
2025-11-13 13:43:08.5422 IST [Polaris Coverity Capture] INFO: npm warn deprecated minimatch@2.0.10: Please update to minimatch 3.0.2 or higher to avoid a RegExp DoS issue
2025-11-13 13:43:08.8350 IST [Polaris Coverity Capture] INFO: npm warn deprecated core-js@1.2.7: core-js@<3.23.3 is no longer maintained and not recommended for usage due to the number of issues. Because of the V8 engine whims, feature detection in old core-js versions could cause a slowdown up to 100x even if nothing is polyfilled. Some versions have web compatibility issues. Please, upgrade your dependencies to the actual version of core-js.
2025-11-13 13:44:34.9783 IST [Polaris Coverity Capture] INFO: 
2025-11-13 13:44:34.9783 IST [Polaris Coverity Capture] INFO: added 737 packages, and audited 738 packages in 3m
2025-11-13 13:44:34.9783 IST [Polaris Coverity Capture] INFO: 
2025-11-13 13:44:34.9783 IST [Polaris Coverity Capture] INFO: 25 packages are looking for funding
2025-11-13 13:44:34.9783 IST [Polaris Coverity Capture] INFO:   run `npm fund` for details
2025-11-13 13:44:35.0164 IST [Polaris Coverity Capture] INFO: 
2025-11-13 13:44:35.0164 IST [Polaris Coverity Capture] INFO: 49 vulnerabilities (1 low, 10 moderate, 19 high, 19 critical)
2025-11-13 13:44:35.0165 IST [Polaris Coverity Capture] INFO: 
2025-11-13 13:44:35.0165 IST [Polaris Coverity Capture] INFO: To address issues that do not require attention, run:
2025-11-13 13:44:35.0165 IST [Polaris Coverity Capture] INFO:   npm audit fix
2025-11-13 13:44:35.0165 IST [Polaris Coverity Capture] INFO: 
2025-11-13 13:44:35.0165 IST [Polaris Coverity Capture] INFO: To address all issues possible (including breaking changes), run:
2025-11-13 13:44:35.0165 IST [Polaris Coverity Capture] INFO:   npm audit fix --force
2025-11-13 13:44:35.0165 IST [Polaris Coverity Capture] INFO: 
2025-11-13 13:44:35.0165 IST [Polaris Coverity Capture] INFO: Some issues need review, and may require choosing
2025-11-13 13:44:35.0165 IST [Polaris Coverity Capture] INFO: a different dependency.
2025-11-13 13:44:35.0165 IST [Polaris Coverity Capture] INFO: 
2025-11-13 13:44:35.0166 IST [Polaris Coverity Capture] INFO: Run `npm audit` for details.
2025-11-13 13:44:35.2756 IST [Polaris Coverity Capture] INFO: Attempting to detect unconfigured compilers in build
2025-11-13 13:44:35.2808 IST [Polaris Coverity Capture] INFO: |0----------25-----------50----------75---------100|
2025-11-13 13:44:35.3894 IST [Polaris Coverity Capture] INFO: ****************************************************
2025-11-13 13:44:35.4163 IST [Polaris Coverity Capture] WARNING: Recorded 0 C/C++ compilation units (0%) successfully. These compilation units are ready for replay
2025-11-13 13:44:35.4164 IST [Polaris Coverity Capture] WARNING: Recoverable errors were encountered during 1 of these C/C++ compilation units.
2025-11-13 13:44:35.4164 IST [Polaris Coverity Capture] INFO: 
2025-11-13 13:44:35.4164 IST [Polaris Coverity Capture] INFO:  For more details, please look at: 
2025-11-13 13:44:35.4164 IST [Polaris Coverity Capture] INFO:     /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/build-log.txt
2025-11-13 13:44:35.4831 IST [Polaris Coverity Capture] INFO: Executing action Collect Build Metrics
2025-11-13 13:44:35.4834 IST [Polaris Coverity Capture] INFO: Executing action Invalidate capture results
2025-11-13 13:44:35.4834 IST [Polaris Coverity Capture] INFO: Executing action Update uncaptured file timestamps for project "/Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/node_modules/consolidate/Makefile"
2025-11-13 13:44:35.4835 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir list-capture-diagnostics
2025-11-13 13:44:36.4892 IST [Polaris Coverity Capture] INFO: Executing action Emit files using buildless capture: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-internal-capture-files --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --ticker-mode none --append-log --capture-list-file /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/capture-file-list-493165409 --record-with-source
2025-11-13 13:44:36.5212 IST [Polaris Coverity Capture] INFO: Buildless capture started.
2025-11-13 13:44:36.5349 IST [Polaris Coverity Capture] INFO: Emitting 84 Files.
2025-11-13 13:44:36.9474 IST [Polaris Coverity Capture] INFO: Buildless capture completed.
2025-11-13 13:44:36.9492 IST [Polaris Coverity Capture] INFO: Executing action Delete unwanted TUs: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit @@/Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/delete-unwanted-tus-action-903897168
2025-11-13 13:44:36.9675 IST [Polaris Coverity Capture] INFO: Executing action Action cleanup: Unwanted TUs action cleanup
2025-11-13 13:44:36.9677 IST [Polaris Coverity Capture] INFO: Executing action deleteResidualTUs /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir
2025-11-13 13:44:36.9680 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir list-capture-diagnostics
2025-11-13 13:44:36.9824 IST [Polaris Coverity Capture] INFO: Executing action Invalidate capture results
2025-11-13 13:44:36.9824 IST [Polaris Coverity Capture] INFO: Executing action Invoke cov-run-sigma: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-run-sigma --project-dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir --coverity-config /var/folders/wm/gkd75sk54h57yqd0_j95gp2r0000gn/T/cov-run-sigma-config-2912935164/coverity.yaml --sigma-binary-path /Users/madhusud/.blackduck/bridge/tools/sigma/2025.10.0/sigma --enable-telemetry
2025-11-13 13:44:37.0184 IST [Polaris Coverity Capture] INFO: cov-run-sigma version 2025.9.0 on Darwin 24.6.0 arm64
2025-11-13 13:44:37.0184 IST [Polaris Coverity Capture] INFO: Internal version numbers: 477d3c5ddd p-2025.9-push-57
2025-11-13 13:44:37.0185 IST [Polaris Coverity Capture] INFO: 
2025-11-13 13:44:38.6603 IST [Polaris Coverity Capture] INFO: Executing action Action cleanup: Coverity configuration for Sigma
2025-11-13 13:44:39.5394 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir list-capture-diagnostics
2025-11-13 13:44:39.6279 IST [Polaris Coverity Capture] INFO: Capture summary:
2025-11-13 13:44:39.6279 IST [Polaris Coverity Capture] INFO:     SUCCEEDED: 87
2025-11-13 13:44:39.6279 IST [Polaris Coverity Capture] INFO:     INCOMPLETE: 0
2025-11-13 13:44:39.6279 IST [Polaris Coverity Capture] INFO:     FAILED: 0
2025-11-13 13:44:39.6280 IST [Polaris Coverity Capture] INFO:     IGNORED: 3
2025-11-13 13:44:39.6280 IST [Polaris Coverity Capture] INFO:     FILES CAPTURED: 87
2025-11-13 13:44:39.6280 IST [Polaris Coverity Capture] INFO:     LINES OF CODE: 32930
2025-11-13 13:44:39.6310 IST [Polaris Coverity Capture] INFO: Capture phase took 2m48.492s.
2025-11-13 13:44:39.6310 IST [Polaris Coverity Capture] WARNING: !! SOURCES FOR UNSUPPORTED LANGUAGES WERE DETECTED !!
2025-11-13 13:44:39.6310 IST [Polaris Coverity Capture] WARNING: 
2025-11-13 13:44:39.6310 IST [Polaris Coverity Capture] WARNING: Source files for the following languages were detected, but these languages are not supported on Mac OS ARM:
2025-11-13 13:44:39.6311 IST [Polaris Coverity Capture] WARNING:   * C#
2025-11-13 13:44:39.6311 IST [Polaris Coverity Capture] WARNING: In order to analyze these files, please analyze the project on an operating system and architecture where they are supported.
2025-11-13 13:44:39.6987 IST [Polaris Coverity Capture] INFO: To analyze your project, type '/Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/coverity analyze --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir -o analyze.location=connect'.
2025-11-13 13:44:39.7013 IST [Polaris Coverity Capture] INFO: Coverity Capture completed successfully
2025-11-13 13:44:39.7083 IST [Polaris Coverity Capture] INFO: Provided value for resource 'coverity.completed'
2025-11-13 13:44:39.7084 IST [Polaris Coverity Capture] INFO: Provided value for resource 'coverity.idir.output'
2025-11-13 13:44:39.7085 IST [Polaris Coverity Capture] INFO: Provided value for resource 'polaris.test.sast.tests.sastFull.artifacts.path'
2025-11-13 13:44:39.7087 IST [Polaris Coverity Capture] INFO: Adapter finished
2025-11-13 13:44:39.7113 IST [Bridge CLI] INFO: Starting Adapter: Default Adapter for execution path
2025-11-13 13:44:39.7114 IST [Default Adapter for execution path] INFO: Provided value for resource 'detect.execution.path'
2025-11-13 13:44:39.7114 IST [Default Adapter for execution path] INFO: Adapter finished
2025-11-13 13:44:39.7474 IST [Polaris SCA Package Manager Scan] INFO: Running command /Library/Java/JavaVirtualMachines/jdk-21.jdk/Contents/Home/bin/java -jar /Users/madhusud/.blackduck/bridge/tools/blackduck-detect/10.4.0/detect-10.4.0.jar --detect.cleanup=false --detect.bdio.file.name=scan --detect.detector.search.depth=3 --detect.bdio.output.path=/Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/bdio/blackduck_artifact --detect.output.path=/Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect --detect.tools=DETECTOR --detect.component.location.analysis.enabled=true --blackduck.offline.mode=true --blackduck.offline.mode.force.bdio=true --detect.diagnostic=true
2025-11-13 13:44:40.0000 IST [Polaris SCA Package Manager Scan][main] WARNING: --- Detect-Self-Updater:  Self-Update feature is disabled because of the following reasons:
2025-11-13 13:44:40.0000 IST [Polaris SCA Package Manager Scan][main] WARNING: --- Detect-Self-Updater:  Detect in offline mode is incompatible with the Self-Update feature.
2025-11-13 13:44:40.0000 IST [Polaris SCA Package Manager Scan][main] WARNING: --- Detect-Self-Updater:  Black Duck URL is required for the Self-Update feature.
2025-11-13 13:44:40.4614 IST [Polaris SCA Package Manager Scan] INFO: ______     _            _
2025-11-13 13:44:40.4615 IST [Polaris SCA Package Manager Scan] INFO: |  _  \   | |          | |
2025-11-13 13:44:40.4615 IST [Polaris SCA Package Manager Scan] INFO: | | | |___| |_ ___  ___| |_
2025-11-13 13:44:40.4615 IST [Polaris SCA Package Manager Scan] INFO: | | | / _ \ __/ _ \/ __| __|
2025-11-13 13:44:40.4615 IST [Polaris SCA Package Manager Scan] INFO: | |/ /  __/ ||  __/ (__| |_
2025-11-13 13:44:40.4615 IST [Polaris SCA Package Manager Scan] INFO: |___/ \___|\__\___|\___|\__|
2025-11-13 13:44:40.4616 IST [Polaris SCA Package Manager Scan] INFO: 
2025-11-13 13:44:40.5773 IST [Polaris SCA Package Manager Scan] INFO: 
2025-11-13 13:44:40.5774 IST [Polaris SCA Package Manager Scan] INFO: Detect Version: 10.4.0
2025-11-13 13:44:40.5774 IST [Polaris SCA Package Manager Scan] INFO: 
2025-11-13 13:44:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 13:44:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Current property values:
2025-11-13 13:44:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- --property = value [notes]
2025-11-13 13:44:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ------------------------------------------------------------
2025-11-13 13:44:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- blackduck.offline.mode = true [cmd] 
2025-11-13 13:44:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- blackduck.offline.mode.force.bdio = true [cmd] 
2025-11-13 13:44:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.bdio.file.name = scan [cmd] 
2025-11-13 13:44:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.bdio.output.path = /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/bdio/blackduck_artifact [cmd] 
2025-11-13 13:44:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.cleanup = false [cmd] 
2025-11-13 13:44:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.component.location.analysis.enabled = true [cmd] 
2025-11-13 13:44:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.detector.search.depth = 3 [cmd] 
2025-11-13 13:44:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.diagnostic = true [cmd] 
2025-11-13 13:44:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.excluded.directories = /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge [env] 
2025-11-13 13:44:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.output.path = /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect [cmd] 
2025-11-13 13:44:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.tools = DETECTOR [cmd] 
2025-11-13 13:44:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ------------------------------------------------------------
2025-11-13 13:44:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 13:44:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Detect build date: 2025-04-24
2025-11-13 13:44:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Source directory: /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm
2025-11-13 13:44:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Output directory: /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect
2025-11-13 13:44:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Run directory: /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-08-14-40-540
2025-11-13 13:44:40.6626 IST [Polaris SCA Package Manager Scan] INFO: 
2025-11-13 13:44:40.6626 IST [Polaris SCA Package Manager Scan] INFO: ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
2025-11-13 13:44:40.6626 IST [Polaris SCA Package Manager Scan] INFO: Diagnostic mode on.
2025-11-13 13:44:40.6626 IST [Polaris SCA Package Manager Scan] INFO: A zip file will be created with logs and relevant Detect output files.
2025-11-13 13:44:40.6626 IST [Polaris SCA Package Manager Scan] INFO: It is generally not recommended to leave diagnostic mode on as you must manually clean up the zip.
2025-11-13 13:44:40.6626 IST [Polaris SCA Package Manager Scan] INFO: ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
2025-11-13 13:44:40.6627 IST [Polaris SCA Package Manager Scan] INFO: 
2025-11-13 13:44:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Initializing diagnostic components.
2025-11-13 13:44:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Created report file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-08-14-40-540/reports/search_report.txt
2025-11-13 13:44:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Created report file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-08-14-40-540/reports/search_detailed_report.txt
2025-11-13 13:44:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Created report file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-08-14-40-540/reports/detector_report.txt
2025-11-13 13:44:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Created report file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-08-14-40-540/reports/detector_profile_report.txt
2025-11-13 13:44:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Created report file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-08-14-40-540/reports/code_location_report.txt
2025-11-13 13:44:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Created report file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-08-14-40-540/reports/dependency_counts_report.txt
2025-11-13 13:44:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Created report file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-08-14-40-540/reports/detect_configuration.txt
2025-11-13 13:44:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Attempting to capture sysout.
2025-11-13 13:44:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Writing sysout to file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-08-14-40-540/logs/sysout.txt
2025-11-13 13:44:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Attempting to set 'com.blackduck.integration' logging level.
2025-11-13 13:44:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Attempting to capture additional log messages to files.
2025-11-13 13:44:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Redirected to file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-08-14-40-540/logs/all.txt
2025-11-13 13:44:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Redirected to file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-08-14-40-540/logs/debug.txt
2025-11-13 13:44:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Redirected to file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-08-14-40-540/logs/info.txt
2025-11-13 13:44:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Attempting to restrict console to debug level (additional levels written to files).
2025-11-13 13:44:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Adding additional log listeners to extractions.
2025-11-13 13:44:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Diagnostics is now in control of logging!
2025-11-13 13:44:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Creating configuration diagnostics reports.
2025-11-13 13:44:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Diagnostics system is ready.
2025-11-13 13:44:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 13:44:40.0000 IST [Polaris SCA Package Manager Scan][main] WARNING: --- Correlated Scanning is not available for Rapid/Stateless scan mode or offline scanning. A correlation ID will not be set.
2025-11-13 13:44:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 13:44:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Docker tool will not be run.
2025-11-13 13:44:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 13:44:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Bazel tool will not be run.
2025-11-13 13:44:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 13:44:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Will include the Detectors tool.
2025-11-13 13:44:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Searching for detectors.
2025-11-13 13:44:40.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Evaluating detectors. This may take a while.
2025-11-13 13:44:41.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ======================================================================================================
2025-11-13 13:44:41.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Detector Report
2025-11-13 13:44:41.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ======================================================================================================
2025-11-13 13:44:41.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 	/Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm (depth 0)
2025-11-13 13:44:41.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 		NPM Package Lock: SUCCESS
2025-11-13 13:44:41.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 			Found file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/package-lock.json
2025-11-13 13:44:41.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 			Found file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/package.json
2025-11-13 13:44:41.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 13:44:41.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Saved file to diagnostics zip: /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/package-lock.json
2025-11-13 13:44:41.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Saved file to diagnostics zip: /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/package.json
2025-11-13 13:44:41.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Detectors actions finished.
2025-11-13 13:44:41.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 13:44:41.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Project name: owasp-nodejs-goat
2025-11-13 13:44:41.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Project version: 1.3.0
2025-11-13 13:44:42.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 13:44:42.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Signature Scanner tool will not be run.
2025-11-13 13:44:42.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 13:44:42.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Vulnerability Impact Analysis tool will not be run.
2025-11-13 13:44:42.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 13:44:42.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- IaC Scanner tool will not be run.
2025-11-13 13:44:43.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 13:44:43.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ##################################################################################################
2025-11-13 13:44:43.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #                                                                                                #
2025-11-13 13:44:43.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  Product Notice                                                                                #
2025-11-13 13:44:43.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  © 2024 Black Duck Software, Inc.                                                              #
2025-11-13 13:44:43.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  This Black Duck Component Locator and all associated documentation are proprietary            #
2025-11-13 13:44:43.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  to Black Duck Software, Inc. and may only be used pursuant to the terms and conditions of a   #
2025-11-13 13:44:43.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  written license agreement with Black Duck Software, Inc. All other use, reproduction,         #
2025-11-13 13:44:43.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  modification, or distribution of the Black Duck Component Locator or the associated           #
2025-11-13 13:44:43.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  documentation is strictly prohibited.                                                         #
2025-11-13 13:44:43.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #                                                                                                #
2025-11-13 13:44:43.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ##################################################################################################
2025-11-13 13:44:43.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Running Component Locator v1.1.12 on /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm
2025-11-13 13:45:45.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Component Location Analysis file saved at: /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-08-14-40-540/scan/components-with-locations.json
2025-11-13 13:45:45.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 13:45:45.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 13:45:45.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 13:45:45.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Creating status file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-08-14-40-540/status/status.json
2025-11-13 13:45:45.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 13:45:45.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Finishing diagnostic mode.
2025-11-13 13:45:45.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Finishing reports.
2025-11-13 13:45:45.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Finishing logging.
2025-11-13 13:45:45.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Finishing executable capture.
2025-11-13 13:45:45.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Finishing file capture.
2025-11-13 13:45:45.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Creating diagnostics zip.
2025-11-13 13:45:45.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Diagnostics zip location: /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/detect-run-2025-11-13-08-14-40-540.zip
2025-11-13 13:45:46.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Diagnostics file created at: /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/detect-run-2025-11-13-08-14-40-540.zip
2025-11-13 13:45:46.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Diagnostic mode has completed.
2025-11-13 13:45:46.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Skipping cleanup, it is disabled.
2025-11-13 13:45:46.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 13:45:46.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 13:45:46.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ======== Detect Result ========
2025-11-13 13:45:46.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 13:45:46.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Component Location Analysis File: /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-08-14-40-540/scan/components-with-locations.json
2025-11-13 13:45:46.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 13:45:46.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ======== Detect Status ========
2025-11-13 13:45:46.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 13:45:46.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- NPM: SUCCESS
2025-11-13 13:45:46.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Overall Status: SUCCESS - Detect exited successfully.
2025-11-13 13:45:46.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 13:45:46.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ===============================
2025-11-13 13:45:46.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 13:45:46.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Detect duration: 00h 01m 06s 019ms
2025-11-13 13:45:46.0980 IST [Polaris SCA Package Manager Scan] INFO: Provided value for resource 'detect.completed'
2025-11-13 13:45:46.0982 IST [Polaris SCA Package Manager Scan] INFO: Provided value for resource 'polaris.test.sca.tests.scaPackage.artifacts.path'
2025-11-13 13:45:46.0984 IST [Polaris SCA Package Manager Scan] INFO: Adapter finished
2025-11-13 13:45:46.1617 IST [Polaris Artifacts Uploader] INFO: uploading artifact for "SAST(sastFull)" assessment with id "ade5b00f-3fbf-4afb-96cc-70943a270bad"
2025-11-13 13:45:46.1623 IST [Polaris Artifacts Uploader] INFO: uploading artifact for "SCA(scaPackage)" assessment with id "10d1042b-ecb7-4533-b0ca-cf46d3d5cb5f"
2025-11-13 13:45:47.7732 IST [Polaris Artifacts Uploader] INFO: Uploading artifact /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_coverity_capture/idir.zip for "SAST(sastFull)" assessment
2025-11-13 13:45:47.7736 IST [Polaris Artifacts Uploader] INFO: Uploading artifact /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/blackduck-sca-artifacts.zip for "SCA(scaPackage)" assessment
2025-11-13 13:45:48.5121 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact:   1%  16384/1543420
2025-11-13 13:45:48.5189 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SCA(scaPackage)" artifact:   6%  16384/235722
2025-11-13 13:45:48.7344 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SCA(scaPackage)" artifact:  34%  81920/235722
2025-11-13 13:45:48.7346 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SCA(scaPackage)" artifact:  62%  147456/235722
2025-11-13 13:45:49.1909 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SCA(scaPackage)" artifact:  90%  212992/235722
2025-11-13 13:45:49.1913 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SCA(scaPackage)" artifact: 100%  235722/235722
2025-11-13 13:45:49.3786 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact:  26%  409600/1543420
2025-11-13 13:45:49.5922 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact:  52%  802816/1543420
2025-11-13 13:45:49.6012 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact:  77%  1196032/1543420
2025-11-13 13:45:49.8267 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact: 100%  1543420/1543420
2025-11-13 13:45:49.8566 IST [Polaris Artifacts Uploader] INFO: successfully uploaded artifact "/Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/blackduck-sca-artifacts.zip"
2025-11-13 13:45:50.3404 IST [Polaris Artifacts Uploader] INFO: successfully uploaded artifact "/Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_coverity_capture/idir.zip"
2025-11-13 13:45:50.3567 IST [Polaris Artifacts Uploader] INFO: successfully resumed "SCA(scaPackage)" assessment with id "10d1042b-ecb7-4533-b0ca-cf46d3d5cb5f"
2025-11-13 13:45:50.7958 IST [Polaris Artifacts Uploader] INFO: successfully resumed "SAST(sastFull)" assessment with id "ade5b00f-3fbf-4afb-96cc-70943a270bad"
2025-11-13 13:45:50.8259 IST [Polaris Artifacts Uploader] INFO: Provided value for resource 'polaris.test.sca.tests.scaPackage.artifacts.uploadSuccessful'
2025-11-13 13:45:50.8261 IST [Polaris Artifacts Uploader] INFO: Provided value for resource 'polaris.test.sast.tests.sastFull.artifacts.uploadSuccessful'
2025-11-13 13:45:50.8264 IST [Polaris Artifacts Uploader] INFO: Adapter finished
2025-11-13 13:45:50.8691 IST [Polaris Waiter] INFO: Waiting for test with assessment type "SAST(sastFull)" and id "ade5b00f-3fbf-4afb-96cc-70943a270bad"
2025-11-13 13:45:50.8695 IST [Polaris Waiter] INFO: Waiting for test with assessment type "SCA(scaPackage)" and id "10d1042b-ecb7-4533-b0ca-cf46d3d5cb5f"
2025-11-13 13:45:51.6321 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SAST(sastFull)" and id "ade5b00f-3fbf-4afb-96cc-70943a270bad" is "Queuing"
2025-11-13 13:45:51.6421 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SCA(scaPackage)" and id "10d1042b-ecb7-4533-b0ca-cf46d3d5cb5f" is "Queuing"
2025-11-13 13:46:01.9560 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SAST(sastFull)" and id "ade5b00f-3fbf-4afb-96cc-70943a270bad" is "Scanning"
2025-11-13 13:46:02.0283 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SCA(scaPackage)" and id "10d1042b-ecb7-4533-b0ca-cf46d3d5cb5f" is "Scanning & Publishing"
2025-11-13 13:46:22.6835 IST [Polaris Waiter] INFO: test with assessment type "SAST(sastFull)" and id "ade5b00f-3fbf-4afb-96cc-70943a270bad" completed successfully
2025-11-13 13:46:22.7210 IST [Polaris Waiter] INFO: test with assessment type "SCA(scaPackage)" and id "10d1042b-ecb7-4533-b0ca-cf46d3d5cb5f" completed successfully
2025-11-13 13:46:22.7442 IST [Polaris Waiter] INFO: Provided value for resource 'polaris.test.sast.tests.sastFull.completed'
2025-11-13 13:46:22.7448 IST [Polaris Waiter] INFO: Provided value for resource 'polaris.test.sca.tests.scaPackage.completed'
2025-11-13 13:46:22.7455 IST [Polaris Waiter] INFO: Adapter finished
2025-11-13 13:46:22.8586 IST [Polaris Issues Fetcher] INFO: Fetching issues for "SCA(scaPackage)" assessment
2025-11-13 13:46:22.8591 IST [Polaris Issues Fetcher] INFO: Fetching issues for "SAST(sastFull)" assessment
2025-11-13 13:46:23.6617 IST [Polaris Issues Fetcher] INFO: Successfully fetched issues for assessment type "SCA(scaPackage)" with id "10d1042b-ecb7-4533-b0ca-cf46d3d5cb5f"
 {
 "critical": 6,
 "high": 109,
 "informational": 0,
 "low": 15,
 "medium": 133
}
2025-11-13 13:46:23.6662 IST [Polaris Issues Fetcher] INFO: Successfully fetched issues for assessment type "SAST(sastFull)" with id "ade5b00f-3fbf-4afb-96cc-70943a270bad"
 {
 "critical": 0,
 "high": 2,
 "informational": 0,
 "low": 25,
 "medium": 13
}
2025-11-13 13:46:23.6925 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.sast.tests.sastFull.issues.medium'
2025-11-13 13:46:23.6929 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.sast.tests.sastFull.issues.low'
2025-11-13 13:46:23.6932 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.sast.tests.sastFull.issues.critical'
2025-11-13 13:46:23.6936 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.sast.tests.sastFull.issues.high'
2025-11-13 13:46:23.6947 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.sast.tests.sastFull.issues.informational'
2025-11-13 13:46:23.6951 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.sca.tests.scaPackage.issues.informational'
2025-11-13 13:46:23.6953 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.sca.tests.scaPackage.issues.medium'
2025-11-13 13:46:23.6956 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.sca.tests.scaPackage.issues.high'
2025-11-13 13:46:23.6958 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.sca.tests.scaPackage.issues.critical'
2025-11-13 13:46:23.6961 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.sca.tests.scaPackage.issues.low'
2025-11-13 13:46:23.6969 IST [Polaris Issues Fetcher] INFO: Adapter finished
2025-11-13 13:46:23.7406 IST [Polaris Policy Checker] INFO: Checking for policy violations for "SAST(sastFull)" assessment...
2025-11-13 13:46:23.7414 IST [Polaris Policy Checker] INFO: Checking for policy violations for "SCA(scaPackage)" assessment...
2025-11-13 13:46:24.6674 IST [Polaris Policy Checker] INFO: no policies were violated to break the build
2025-11-13 13:46:24.6899 IST [Polaris Policy Checker] INFO: Adapter finished
2025-11-13 13:46:24.7435 IST [Polaris SARIF Issues Fetcher] INFO: Fetching issues from Polaris Server...
2025-11-13 13:47:27.5681 IST [Polaris SARIF Issues Fetcher] INFO: Added entry to resource 'polaris.reports.sarif.issues'
2025-11-13 13:47:27.5738 IST [Bridge CLI] INFO: Starting adapters for stage polaris-sarif-generator
2025-11-13 13:47:27.5739 IST [Bridge CLI] INFO: Starting Adapter: Polaris SARIF Generator
2025-11-13 13:47:27.5741 IST [Polaris SARIF Issues Fetcher] INFO: Adapter finished
2025-11-13 13:47:27.6257 IST [Polaris Status Provider] INFO: Results for test "SAST(sastFull)" with ID "ade5b00f-3fbf-4afb-96cc-70943a270bad" are available at https://poc.polaris.blackduck.com/portfolio/portfolios/edf596d3-b54f-4a6b-9e5c-209f2e526c67/portfolio-items/8a1259ec-ad21-47ce-a755-cb6d96d9f329/projects/77fd4955-2c78-49c2-bab5-680ed8575b99/tests/ade5b00f-3fbf-4afb-96cc-70943a270bad/detected-issues
2025-11-13 13:47:27.6260 IST [Polaris Status Provider] INFO: Results for test "SCA(scaPackage)" with ID "10d1042b-ecb7-4533-b0ca-cf46d3d5cb5f" are available at https://poc.polaris.blackduck.com/portfolio/portfolios/edf596d3-b54f-4a6b-9e5c-209f2e526c67/portfolio-items/8a1259ec-ad21-47ce-a755-cb6d96d9f329/projects/77fd4955-2c78-49c2-bab5-680ed8575b99/tests/10d1042b-ecb7-4533-b0ca-cf46d3d5cb5f/detected-issues
2025-11-13 13:47:27.6260 IST [Polaris Status Provider] INFO: Polaris issues view for project "detailed-example", branch "main" is available at https://poc.polaris.blackduck.com/portfolio/portfolios/edf596d3-b54f-4a6b-9e5c-209f2e526c67/portfolio-items/8a1259ec-ad21-47ce-a755-cb6d96d9f329/projects/77fd4955-2c78-49c2-bab5-680ed8575b99/issues?branchId=c9a05d59-6c9c-4ae1-8661-61d6a38179cb
2025-11-13 13:47:27.6333 IST [Polaris Status Provider] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.summary.url'
2025-11-13 13:47:27.6334 IST [Polaris Status Provider] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.summary.url'
2025-11-13 13:47:27.6336 IST [Polaris Status Provider] INFO: Provided value for resource 'polaris.project.issues.url'
2025-11-13 13:47:27.6343 IST [Polaris Status Provider] INFO: Adapter finished
2025-11-13 13:47:27.6752 IST [Polaris SARIF Generator] INFO: Will create rules with SCA component-version pairs grouped by their related vulnerabilities in the SARIF report. Since "polaris.reports.sarif.groupSCAIssues" is configured to "true"
2025-11-13 13:47:27.6793 IST [Polaris SARIF Generator] INFO: SARIF report created successfully at .blackduck/integrations/polaris/sarif/report.sarif.json
2025-11-13 13:47:27.6961 IST [Polaris SARIF Generator] INFO: Provided value for resource 'polaris.reports.sarif.file.output'
2025-11-13 13:47:27.6964 IST [Polaris SARIF Generator] INFO: Adapter finished
******************************* END EXECUTION OF BRIDGE CLI *******************************
[Security Scan] INFO: This is not a (PR/MR) event
[Security Scan] INFO: Archiving SARIF jenkins artifact from: /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.blackduck/integrations/polaris/sarif/report.sarif.json
Archiving artifacts
[Security Scan] INFO: SARIF archived successfully in jenkins artifact
[Security Scan] INFO: Retrieving the issue count from the scan results
[Security Scan] INFO: Total issues found: 303
[Security Scan] INFO: Security Scan execution is successful
**************************** END EXECUTION OF BLACK DUCK SECURITY SCAN ****************************
[Pipeline] }
[Pipeline] // dir
[Pipeline] }
[Pipeline] // script
[Pipeline] }
[Pipeline] // stage
[Pipeline] stage
[Pipeline] { (Declarative: Post Actions)
[Pipeline] echo
Black Duck Logs Publisher - Starting log upload process
[Pipeline] echo
Configuration: [githubOrg:polaris-jenkins-samples, repoName:detailed-example, credentialsId:github-pat-logs-publisher, maxRetries:3, retentionCount:5, jobNamePrefixes:[MBP_Github_, MBP_, Github_, Pipeline_, Job_, Build_]]
[Pipeline] echo
Job Name: MBP_Github_Polaris_Detailed_Workflow/main
[Pipeline] echo
Build Number: 2
[Pipeline] echo
GitHub Organization: polaris-jenkins-samples
[Pipeline] withCredentials
Masking supported pattern matches of $GITHUB_TOKEN
[Pipeline] {
[Pipeline] echo
Using configured repository name: detailed-example
[Pipeline] echo
Target repository: polaris-jenkins-samples/detailed-example
[Pipeline] echo
LogProcessor: captureJenkinsLogs called
```

---

*Log generated by Black Duck Logs Publisher*