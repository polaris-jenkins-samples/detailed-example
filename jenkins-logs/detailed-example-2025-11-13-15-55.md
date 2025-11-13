# Jenkins Execution Log

## Build Information
- **Job Name:** `MBP_Github_Polaris_Detailed_Workflow/main`
- **Build Number:** #3
- **Build Status:** 🟢 **SUCCESS**
- **Duration:** 4 min 38 sec and counting
- **Timestamp:** 2025-11-13 15:55:29 UTC

---

## Console Output

```
Started by user admin
Connecting to https://api.github.com using madhusud@blackduck.com/****** (Github_Username_PAT)
Obtained nodejs-npm/Jenkinsfile from 548b281a15f4398f305f70d011a7e5cff231b634
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
Checking out Revision 548b281a15f4398f305f70d011a7e5cff231b634 (main)
Commit message: "Delete jenkins-logs directory"
 > git config core.sparsecheckout # timeout=10
 > git checkout -f 548b281a15f4398f305f70d011a7e5cff231b634 # timeout=10
 > git rev-list --no-walk 0ccd1a0edec3703eaacff39616ccb574f0e694d7 # timeout=10
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

removed 737 packages, and audited 1412 packages in 24s

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
[Security Scan] INFO: Executable command line arguments: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm/bridge-cli --stage polaris --input /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/polaris_input14027613737588894693.json --out .bridge/output/scan_info_out.json

******************************* START EXECUTION OF BRIDGE CLI *******************************
2025-11-13 15:51:32.4856 IST [Bridge CLI] INFO: Using cache directory: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm
2025-11-13 15:51:32.5043 IST [Bridge CLI] INFO: Found version "3.0.371" in registry for workflow "polaris", trying to load it from local cache
2025-11-13 15:51:33.8174 IST [Bridge CLI] INFO: Input Resources:
2025-11-13 15:51:33.8175 IST [Bridge CLI] INFO: resource = value [source]
2025-11-13 15:51:33.8175 IST [Bridge CLI] INFO: ------------------------------------------------------------
2025-11-13 15:51:33.8175 IST [Bridge CLI] INFO: coverity.build.command = npm install [polaris_input14027613737588894693.json]
2025-11-13 15:51:33.8175 IST [Bridge CLI] INFO: coverity.clean.command = npm cache clean --force [polaris_input14027613737588894693.json]
2025-11-13 15:51:33.8175 IST [Bridge CLI] INFO: detect.args = --detect.diagnostic=true [polaris_input14027613737588894693.json]
2025-11-13 15:51:33.8175 IST [Bridge CLI] INFO: detect.search.depth = 3 [polaris_input14027613737588894693.json]
2025-11-13 15:51:33.8175 IST [Bridge CLI] INFO: network.airgap = false [polaris_input14027613737588894693.json]
2025-11-13 15:51:33.8175 IST [Bridge CLI] INFO: polaris.accesstoken = ***************************************** [polaris_input14027613737588894693.json]
2025-11-13 15:51:33.8175 IST [Bridge CLI] INFO: polaris.application.name = detailed-example [polaris_input14027613737588894693.json]
2025-11-13 15:51:33.8176 IST [Bridge CLI] INFO: polaris.assessment.types = [SAST SCA] [polaris_input14027613737588894693.json]
2025-11-13 15:51:33.8176 IST [Bridge CLI] INFO: polaris.branch.name = main [polaris_input14027613737588894693.json]
2025-11-13 15:51:33.8176 IST [Bridge CLI] INFO: polaris.project.name = detailed-example [polaris_input14027613737588894693.json]
2025-11-13 15:51:33.8176 IST [Bridge CLI] INFO: polaris.reports.sarif.create = true [polaris_input14027613737588894693.json]
2025-11-13 15:51:33.8176 IST [Bridge CLI] INFO: polaris.reports.sarif.file.path = .blackduck/integrations/polaris/sarif/report.sarif.json [polaris_input14027613737588894693.json]
2025-11-13 15:51:33.8176 IST [Bridge CLI] INFO: polaris.reports.sarif.groupSCAIssues = true [polaris_input14027613737588894693.json]
2025-11-13 15:51:33.8176 IST [Bridge CLI] INFO: polaris.reports.sarif.issue.types = [SAST SCA] [polaris_input14027613737588894693.json]
2025-11-13 15:51:33.8176 IST [Bridge CLI] INFO: polaris.reports.sarif.severities = [CRITICAL HIGH] [polaris_input14027613737588894693.json]
2025-11-13 15:51:33.8176 IST [Bridge CLI] INFO: polaris.serverUrl = https://poc.polaris.blackduck.com [polaris_input14027613737588894693.json]
2025-11-13 15:51:33.8176 IST [Bridge CLI] INFO: polaris.test.sast.location = hybrid [polaris_input14027613737588894693.json]
2025-11-13 15:51:33.8176 IST [Bridge CLI] INFO: polaris.test.sca.location = hybrid [polaris_input14027613737588894693.json]
2025-11-13 15:51:33.8176 IST [Bridge CLI] INFO: polaris.waitForScan = true [polaris_input14027613737588894693.json]
2025-11-13 15:51:33.8176 IST [Bridge CLI] INFO: ------------------------------------------------------------
2025-11-13 15:51:33.8176 IST [Bridge CLI] INFO: Starting adapters for stage polaris
2025-11-13 15:51:33.8193 IST [Bridge CLI] INFO: Starting Adapter: Polaris Status Provider
2025-11-13 15:51:33.8194 IST [Bridge CLI] INFO: Starting Adapter: Polaris Controller
2025-11-13 15:51:33.8194 IST [Bridge CLI] INFO: Starting Adapter: Polaris Initializer
2025-11-13 15:51:33.8194 IST [Bridge CLI] INFO: Starting Adapter: Polaris SCM Discovery
2025-11-13 15:51:33.9215 IST [Polaris SCM Discovery] INFO: Adapter finished
2025-11-13 15:51:33.9263 IST [Bridge CLI] INFO: Starting Adapter: Set Polaris Assessment Mode to CI
2025-11-13 15:51:33.9265 IST [Set Polaris Assessment Mode to CI] INFO: Provided value for resource 'polaris.assessment.mode'
2025-11-13 15:51:33.9265 IST [Set Polaris Assessment Mode to CI] INFO: Adapter finished
2025-11-13 15:51:33.9308 IST [Bridge CLI] INFO: Starting Adapter: Create Polaris Project & Branch By Default
2025-11-13 15:51:33.9309 IST [Create Polaris Project & Branch By Default] INFO: Provided value for resource 'polaris.onboarding'
2025-11-13 15:51:33.9309 IST [Create Polaris Project & Branch By Default] INFO: Adapter finished
2025-11-13 15:51:36.5900 IST [Polaris Initializer] INFO: Successfully created test for "SAST(sastFull)" assessment. The short test ID is "X83IBUQ"
2025-11-13 15:51:36.6406 IST [Polaris Initializer] INFO: Successfully created test for "SCA(scaPackage)" assessment. The short test ID is "OWG3LK4"
2025-11-13 15:51:36.6713 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.id'
2025-11-13 15:51:36.6716 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.id'
2025-11-13 15:51:36.6719 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.shortId'
2025-11-13 15:51:36.6722 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.shortId'
2025-11-13 15:51:36.6725 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.streamId'
2025-11-13 15:51:36.6728 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.project.id'
2025-11-13 15:51:36.6730 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.branch.id'
2025-11-13 15:51:36.6732 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.portfolioid'
2025-11-13 15:51:36.6734 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.tenant.id'
2025-11-13 15:51:36.6737 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.application.id'
2025-11-13 15:51:36.6752 IST [Polaris Initializer] INFO: Adapter finished
2025-11-13 15:51:36.6912 IST [Bridge CLI] INFO: Starting Adapter: Check pull request
2025-11-13 15:51:36.7315 IST [Check pull request] INFO: Provided value for resource 'environment.scan.pull'
2025-11-13 15:51:36.7317 IST [Check pull request] INFO: Adapter finished
2025-11-13 15:51:36.7783 IST [Polaris Controller] INFO: Running for "sast" assessment with scan type "sastFull"
2025-11-13 15:51:36.7788 IST [Polaris Controller] INFO: fetching recommended "coverity" tool info...
2025-11-13 15:51:37.5310 IST [Polaris Controller] INFO: checking "coverity" tool installation inside bridge home directory: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0
2025-11-13 15:51:37.5313 IST [Polaris Controller] INFO: Checking tool version for "cov_thin_client" in "/Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0"
2025-11-13 15:51:37.5316 IST [Polaris Controller] INFO: Running command:/Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/coverity --version
2025-11-13 15:51:37.6025 IST [Polaris Controller] INFO: Got tool version for "cov_thin_client": 2025.9.0
2025-11-13 15:51:37.8893 IST [Polaris Controller] INFO: "coverity" tool is already installed...
2025-11-13 15:51:37.8896 IST [Polaris Controller] INFO: fetching recommended "Sigma" tool info...
2025-11-13 15:51:38.1736 IST [Polaris Controller] INFO: checking "Sigma" tool installation inside bridge home directory: /Users/madhusud/.blackduck/bridge/tools/sigma/2025.10.0
2025-11-13 15:51:38.1740 IST [Polaris Controller] INFO: Checking tool version for "sigma" in "/Users/madhusud/.blackduck/bridge/tools/sigma/2025.10.0"
2025-11-13 15:51:38.1742 IST [Polaris Controller] INFO: Running command:/Users/madhusud/.blackduck/bridge/tools/sigma/2025.10.0/sigma --version
2025-11-13 15:51:38.2797 IST [Polaris Controller] INFO: Got tool version for "sigma": 2025.10.0
2025-11-13 15:51:38.5718 IST [Polaris Controller] INFO: "Sigma" tool is already installed...
2025-11-13 15:51:38.5719 IST [Polaris Controller] INFO: Running for "sca" assessment with scan type "scaPackage"
2025-11-13 15:51:38.5720 IST [Polaris Controller] INFO: fetching recommended "detect" tool info...
2025-11-13 15:51:38.8803 IST [Polaris Controller] INFO: checking "detect" tool installation inside bridge home directory: /Users/madhusud/.blackduck/bridge/tools/blackduck-detect/10.4.0
2025-11-13 15:51:38.8805 IST [Polaris Controller] INFO: Running command:/Library/Java/JavaVirtualMachines/jdk-21.jdk/Contents/Home/bin/java -version
2025-11-13 15:51:38.9637 IST [Polaris Controller] INFO: Checking tool version for "detect" in "/Users/madhusud/.blackduck/bridge/tools/blackduck-detect/10.4.0"
2025-11-13 15:51:38.9670 IST [Polaris Controller] INFO: Got tool version for "detect": 10.4.0
2025-11-13 15:51:39.2484 IST [Polaris Controller] INFO: "detect" tool is already installed...
2025-11-13 15:51:39.2801 IST [Polaris Controller] INFO: Provided value for resource 'coverity.id'
2025-11-13 15:51:39.2804 IST [Polaris Controller] INFO: Provided value for resource 'sigma.id'
2025-11-13 15:51:39.2807 IST [Polaris Controller] INFO: Provided value for resource 'detect.id'
2025-11-13 15:51:39.2808 IST [Bridge CLI] INFO: Starting adapters for stage polaris-sast
2025-11-13 15:51:39.2808 IST [Bridge CLI] INFO: Starting adapters for stage polaris-sca-package
2025-11-13 15:51:39.2808 IST [Bridge CLI] INFO: Starting adapters for stage polaris-artifacts-uploader
2025-11-13 15:51:39.2808 IST [Bridge CLI] INFO: Starting adapters for stage polaris-post-processing
2025-11-13 15:51:39.2808 IST [Bridge CLI] INFO: Starting adapters for stage polaris-reports-sarif
2025-11-13 15:51:39.2838 IST [Bridge CLI] INFO: Starting Adapter: Polaris SCA Package Manager Scan
2025-11-13 15:51:39.2838 IST [Bridge CLI] INFO: Starting Adapter: Polaris Coverity Capture
2025-11-13 15:51:39.2838 IST [Bridge CLI] INFO: Starting Adapter: Polaris Artifacts Uploader
2025-11-13 15:51:39.2838 IST [Bridge CLI] INFO: Starting Adapter: Polaris Waiter
2025-11-13 15:51:39.2838 IST [Bridge CLI] INFO: Starting Adapter: Polaris Issues Fetcher
2025-11-13 15:51:39.2838 IST [Bridge CLI] INFO: Starting Adapter: Polaris Policy Checker
2025-11-13 15:51:39.2838 IST [Bridge CLI] INFO: Starting Adapter: Polaris SARIF Issues Fetcher
2025-11-13 15:51:39.2847 IST [Polaris Controller] INFO: Adapter finished
2025-11-13 15:51:39.3271 IST [Bridge CLI] INFO: Starting Adapter: Default Adapter for execution path
2025-11-13 15:51:39.3275 IST [Default Adapter for execution path] INFO: Provided value for resource 'coverity.execution.path'
2025-11-13 15:51:39.3276 IST [Default Adapter for execution path] INFO: Adapter finished
2025-11-13 15:51:39.3446 IST [Bridge CLI] INFO: Starting Adapter: Default Adapter for execution path
2025-11-13 15:51:39.3448 IST [Default Adapter for execution path] INFO: Provided value for resource 'sigma.execution.path'
2025-11-13 15:51:39.3448 IST [Default Adapter for execution path] INFO: Adapter finished
2025-11-13 15:51:39.4140 IST [Polaris Coverity Capture] INFO: Identified workflow: Polaris
2025-11-13 15:51:39.4149 IST [Polaris Coverity Capture] INFO: command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/coverity capture --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir -o capture.build.clean-command=npm cache clean --force -o analyze.location=connect -- npm install
2025-11-13 15:51:39.4841 IST [Polaris Coverity Capture] INFO: coverity 2025.9.0 covcli-2025.9-push-12
2025-11-13 15:51:39.4842 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CACHE_API_TOKEN_FILE=/var/folders/wm/gkd75sk54h57yqd0_j95gp2r0000gn/T/polaris_coverity_cache3983714326/.authKey
2025-11-13 15:51:39.4842 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CACHE_KEY=ceac6937-e678-4b1e-9838-f1a4cdc36d87
2025-11-13 15:51:39.4842 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CACHE_URL=https://poc.polaris.blackduck.com/api/cache
2025-11-13 15:51:39.4842 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CLI_CAPTURE_ZIP_ARCHIVE=/Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_coverity_capture/idir.zip
2025-11-13 15:51:39.4842 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CLI_POLARIS_CLIENT=true
2025-11-13 15:51:39.4887 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir reset-host-name
2025-11-13 15:51:39.5375 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir check-compatible
2025-11-13 15:51:39.5691 IST [Polaris Coverity Capture] INFO: Detected that stdout is not connected to a terminal.  Defaulting ticker mode to 'none'.
2025-11-13 15:51:39.5691 IST [Polaris Coverity Capture] INFO: If this is not correct, explicitly set the ticker mode to the desired value using the '--ticker-mode' option.
2025-11-13 15:51:39.5705 IST [Polaris Coverity Capture] INFO: Using lightweight capture with thin client.
2025-11-13 15:51:39.5707 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-internal-manage-cache check
2025-11-13 15:51:40.3980 IST [Polaris Coverity Capture] INFO: Caching is enabled.
2025-11-13 15:51:40.4010 IST [Polaris Coverity Capture] INFO: Telemetry is enabled
2025-11-13 15:51:41.4172 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir list-capture-diagnostics
2025-11-13 15:51:41.4419 IST [Polaris Coverity Capture] INFO: Executing action no-op: nothing to do for initialization
2025-11-13 15:51:41.8939 IST [Polaris Coverity Capture] INFO: Executing action no-op: skipping compiler configuration
2025-11-13 15:51:42.3160 IST [Polaris Coverity Capture] INFO: Executing action no-op: no compilers need to be unconfigured
2025-11-13 15:51:42.7375 IST [Polaris Coverity Capture] INFO: Executing action no-op: compiler configurations loaded
2025-11-13 15:51:43.2130 IST [Polaris Coverity Capture] INFO: Executing action Execute clean command: sh -c npm cache clean --force
2025-11-13 15:51:43.3613 IST [Polaris Coverity Capture] INFO: npm warn using --force Recommended protections disabled.
2025-11-13 15:51:44.2301 IST [Polaris Coverity Capture] INFO: Executing action Invoke build capture: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-build --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --append-log --no-security-da --record-with-source --no-xrefs --enable-scan-transparency-data --bytecode-caching npm install
2025-11-13 15:51:44.2708 IST [Polaris Coverity Capture] INFO: Coverity Build Capture (64-bit) version 2025.9.0 on Darwin 24.6.0 arm64
2025-11-13 15:51:44.2709 IST [Polaris Coverity Capture] INFO: Internal version numbers: 477d3c5ddd p-2025.9-push-57
2025-11-13 15:51:44.2709 IST [Polaris Coverity Capture] INFO: 
2025-11-13 15:51:44.2847 IST [Polaris Coverity Capture] INFO: 
2025-11-13 15:51:50.7930 IST [Polaris Coverity Capture] INFO: npm warn deprecated urix@0.1.0: Please see https://github.com/lydell/urix#deprecated
2025-11-13 15:51:51.0144 IST [Polaris Coverity Capture] INFO: npm warn deprecated try-resolve@1.0.1: Package no longer supported. Contact Support at https://www.npmjs.com/support for more info.
2025-11-13 15:51:51.0304 IST [Polaris Coverity Capture] INFO: npm warn deprecated transformers@2.1.0: Deprecated, use jstransformer
2025-11-13 15:51:51.3471 IST [Polaris Coverity Capture] INFO: npm warn deprecated swig@1.4.2: This package is no longer maintained
2025-11-13 15:51:51.5494 IST [Polaris Coverity Capture] INFO: npm warn deprecated stable@0.1.8: Modern JS already guarantees Array#sort() is a stable sort, so this library is deprecated. See the compatibility table on MDN: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/sort#browser_compatibility
2025-11-13 15:51:51.6756 IST [Polaris Coverity Capture] INFO: npm warn deprecated source-map-url@0.4.1: See https://github.com/lydell/source-map-url#deprecated
2025-11-13 15:51:51.6826 IST [Polaris Coverity Capture] INFO: npm warn deprecated source-map-resolve@0.5.3: See https://github.com/lydell/source-map-resolve#deprecated
2025-11-13 15:51:52.2409 IST [Polaris Coverity Capture] INFO: npm warn deprecated resolve-url@0.2.1: https://github.com/lydell/resolve-url#deprecated
2025-11-13 15:51:52.2517 IST [Polaris Coverity Capture] INFO: npm warn deprecated rimraf@2.6.3: Rimraf versions prior to v4 are no longer supported
2025-11-13 15:51:52.8900 IST [Polaris Coverity Capture] INFO: npm warn deprecated q@0.8.12: You or someone you depend on is using Q, the JavaScript Promise library that gave JavaScript developers strong feelings about promises. They can almost certainly migrate to the native JavaScript promise now. Thank you literally everyone for joining me in this bet against the odds. Be excellent to each other.
2025-11-13 15:51:52.8901 IST [Polaris Coverity Capture] INFO: npm warn deprecated
2025-11-13 15:51:52.8901 IST [Polaris Coverity Capture] INFO: npm warn deprecated (For a CapTP with native promises, see @endo/eventual-send and @endo/captp)
2025-11-13 15:51:54.7589 IST [Polaris Coverity Capture] INFO: npm warn deprecated json3@3.3.2: Please use the native JSON object instead of JSON 3
2025-11-13 15:51:54.9551 IST [Polaris Coverity Capture] INFO: npm warn deprecated jade@1.11.0: Jade has been renamed to pug, please install the latest version of pug instead of jade
2025-11-13 15:51:55.5228 IST [Polaris Coverity Capture] INFO: npm warn deprecated inflight@1.0.6: This module is not supported, and leaks memory. Do not use it. Check out lru-cache if you want a good and tested way to coalesce async requests by a key value, which is much more comprehensive and powerful.
2025-11-13 15:51:56.0416 IST [Polaris Coverity Capture] INFO: npm warn deprecated glob@7.2.3: Glob versions prior to v9 are no longer supported
2025-11-13 15:51:56.9830 IST [Polaris Coverity Capture] INFO: npm warn deprecated eslint@3.19.0: This version is no longer supported. Please see https://eslint.org/version-support for other options.
2025-11-13 15:51:57.6236 IST [Polaris Coverity Capture] INFO: npm warn deprecated constantinople@3.0.2: Please update to at least constantinople 3.1.1
2025-11-13 15:51:57.7202 IST [Polaris Coverity Capture] INFO: npm warn deprecated core-js@2.6.12: core-js@<3.23.3 is no longer maintained and not recommended for usage due to the number of issues. Because of the V8 engine whims, feature detection in old core-js versions could cause a slowdown up to 100x even if nothing is polyfilled. Some versions have web compatibility issues. Please, upgrade your dependencies to the actual version of core-js.
2025-11-13 15:51:57.7468 IST [Polaris Coverity Capture] INFO: npm warn deprecated coffee-script@1.12.7: CoffeeScript on NPM has moved to "coffeescript" (no hyphen)
2025-11-13 15:51:57.8922 IST [Polaris Coverity Capture] INFO: npm warn deprecated circular-json@0.3.3: CircularJSON is in maintenance only, flatted is its successor.
2025-11-13 15:51:58.4414 IST [Polaris Coverity Capture] INFO: npm warn deprecated babel-plugin-undefined-to-void@1.1.6: Package no longer supported. Contact Support at https://www.npmjs.com/support for more info.
2025-11-13 15:51:58.6025 IST [Polaris Coverity Capture] INFO: npm warn deprecated babel-plugin-runtime@1.0.7: Package no longer supported. Contact Support at https://www.npmjs.com/support for more info.
2025-11-13 15:51:58.6042 IST [Polaris Coverity Capture] INFO: npm warn deprecated babel-plugin-remove-debugger@1.0.1: Package no longer supported. Contact Support at https://www.npmjs.com/support for more info.
2025-11-13 15:51:58.6422 IST [Polaris Coverity Capture] INFO: npm warn deprecated babel-plugin-remove-console@1.0.1: Package no longer supported. Contact Support at https://www.npmjs.com/support for more info.
2025-11-13 15:51:58.6508 IST [Polaris Coverity Capture] INFO: npm warn deprecated babel-plugin-react-display-name@1.0.3: Package no longer supported. Contact Support at https://www.npmjs.com/support for more info.
2025-11-13 15:51:58.6549 IST [Polaris Coverity Capture] INFO: npm warn deprecated babel-plugin-proto-to-assign@1.0.4: Package no longer supported. Contact Support at https://www.npmjs.com/support for more info.
2025-11-13 15:51:58.7060 IST [Polaris Coverity Capture] INFO: npm warn deprecated babel-plugin-property-literals@1.0.1: Package no longer supported. Contact Support at https://www.npmjs.com/support for more info.
2025-11-13 15:51:58.7063 IST [Polaris Coverity Capture] INFO: npm warn deprecated babel-plugin-jscript@1.0.4: Package no longer supported. Contact Support at https://www.npmjs.com/support for more info.
2025-11-13 15:51:58.7065 IST [Polaris Coverity Capture] INFO: npm warn deprecated babel-plugin-react-constant-elements@1.0.3: Package no longer supported. Contact Support at https://www.npmjs.com/support for more info.
2025-11-13 15:51:58.7100 IST [Polaris Coverity Capture] INFO: npm warn deprecated babel-plugin-inline-environment-variables@1.0.1: Package no longer supported. Contact Support at https://www.npmjs.com/support for more info.
2025-11-13 15:51:58.7752 IST [Polaris Coverity Capture] INFO: npm warn deprecated babel-plugin-member-expression-literals@1.0.1: Package no longer supported. Contact Support at https://www.npmjs.com/support for more info.
2025-11-13 15:51:58.7774 IST [Polaris Coverity Capture] INFO: npm warn deprecated babel-plugin-constant-folding@1.0.1: Package no longer supported. Contact Support at https://www.npmjs.com/support for more info.
2025-11-13 15:51:58.7912 IST [Polaris Coverity Capture] INFO: npm warn deprecated babel-plugin-eval@1.0.1: Package no longer supported. Contact Support at https://www.npmjs.com/support for more info.
2025-11-13 15:51:58.8814 IST [Polaris Coverity Capture] INFO: npm warn deprecated babel-plugin-dead-code-elimination@1.0.2: Package no longer supported. Contact Support at https://www.npmjs.com/support for more info.
2025-11-13 15:52:00.1784 IST [Polaris Coverity Capture] INFO: npm warn deprecated q@1.5.1: You or someone you depend on is using Q, the JavaScript Promise library that gave JavaScript developers strong feelings about promises. They can almost certainly migrate to the native JavaScript promise now. Thank you literally everyone for joining me in this bet against the odds. Be excellent to each other.
2025-11-13 15:52:00.1785 IST [Polaris Coverity Capture] INFO: npm warn deprecated
2025-11-13 15:52:00.1785 IST [Polaris Coverity Capture] INFO: npm warn deprecated (For a CapTP with native promises, see @endo/eventual-send and @endo/captp)
2025-11-13 15:52:00.6702 IST [Polaris Coverity Capture] INFO: npm warn deprecated mkdirp@0.5.1: Legacy versions of mkdirp are no longer supported. Please update to mkdirp 1.x. (Note that the API surface has changed to use Promises in 1.x.)
2025-11-13 15:52:00.6830 IST [Polaris Coverity Capture] INFO: npm warn deprecated glob@7.1.1: Glob versions prior to v9 are no longer supported
2025-11-13 15:52:01.1406 IST [Polaris Coverity Capture] INFO: npm warn deprecated minimatch@0.3.0: Please update to minimatch 3.0.2 or higher to avoid a RegExp DoS issue
2025-11-13 15:52:01.1417 IST [Polaris Coverity Capture] INFO: npm warn deprecated mkdirp@0.3.0: Legacy versions of mkdirp are no longer supported. Please update to mkdirp 1.x. (Note that the API surface has changed to use Promises in 1.x.)
2025-11-13 15:52:01.3997 IST [Polaris Coverity Capture] INFO: npm warn deprecated glob@3.2.11: Glob versions prior to v9 are no longer supported
2025-11-13 15:52:01.5849 IST [Polaris Coverity Capture] INFO: npm warn deprecated core-js@1.2.7: core-js@<3.23.3 is no longer maintained and not recommended for usage due to the number of issues. Because of the V8 engine whims, feature detection in old core-js versions could cause a slowdown up to 100x even if nothing is polyfilled. Some versions have web compatibility issues. Please, upgrade your dependencies to the actual version of core-js.
2025-11-13 15:52:01.8143 IST [Polaris Coverity Capture] INFO: npm warn deprecated fsevents@1.2.13: Upgrade to fsevents v2 to mitigate potential security issues
2025-11-13 15:52:02.1273 IST [Polaris Coverity Capture] INFO: npm warn deprecated q@1.5.1: You or someone you depend on is using Q, the JavaScript Promise library that gave JavaScript developers strong feelings about promises. They can almost certainly migrate to the native JavaScript promise now. Thank you literally everyone for joining me in this bet against the odds. Be excellent to each other.
2025-11-13 15:52:02.1273 IST [Polaris Coverity Capture] INFO: npm warn deprecated
2025-11-13 15:52:02.1273 IST [Polaris Coverity Capture] INFO: npm warn deprecated (For a CapTP with native promises, see @endo/eventual-send and @endo/captp)
2025-11-13 15:52:02.2563 IST [Polaris Coverity Capture] INFO: npm warn deprecated glob@5.0.15: Glob versions prior to v9 are no longer supported
2025-11-13 15:52:02.8085 IST [Polaris Coverity Capture] INFO: npm warn deprecated minimatch@2.0.10: Please update to minimatch 3.0.2 or higher to avoid a RegExp DoS issue
2025-11-13 15:52:02.8791 IST [Polaris Coverity Capture] INFO: npm warn deprecated core-js@1.2.7: core-js@<3.23.3 is no longer maintained and not recommended for usage due to the number of issues. Because of the V8 engine whims, feature detection in old core-js versions could cause a slowdown up to 100x even if nothing is polyfilled. Some versions have web compatibility issues. Please, upgrade your dependencies to the actual version of core-js.
2025-11-13 15:52:03.0315 IST [Polaris Coverity Capture] INFO: npm warn deprecated core-js@1.2.7: core-js@<3.23.3 is no longer maintained and not recommended for usage due to the number of issues. Because of the V8 engine whims, feature detection in old core-js versions could cause a slowdown up to 100x even if nothing is polyfilled. Some versions have web compatibility issues. Please, upgrade your dependencies to the actual version of core-js.
2025-11-13 15:52:21.7438 IST [Polaris Coverity Capture] INFO: 
2025-11-13 15:52:21.7438 IST [Polaris Coverity Capture] INFO: added 738 packages, and audited 739 packages in 33s
2025-11-13 15:52:21.7438 IST [Polaris Coverity Capture] INFO: 
2025-11-13 15:52:21.7438 IST [Polaris Coverity Capture] INFO: 25 packages are looking for funding
2025-11-13 15:52:21.7439 IST [Polaris Coverity Capture] INFO:   run `npm fund` for details
2025-11-13 15:52:21.7843 IST [Polaris Coverity Capture] INFO: 
2025-11-13 15:52:21.7843 IST [Polaris Coverity Capture] INFO: 49 vulnerabilities (1 low, 9 moderate, 21 high, 18 critical)
2025-11-13 15:52:21.7843 IST [Polaris Coverity Capture] INFO: 
2025-11-13 15:52:21.7843 IST [Polaris Coverity Capture] INFO: To address issues that do not require attention, run:
2025-11-13 15:52:21.7843 IST [Polaris Coverity Capture] INFO:   npm audit fix
2025-11-13 15:52:21.7843 IST [Polaris Coverity Capture] INFO: 
2025-11-13 15:52:21.7843 IST [Polaris Coverity Capture] INFO: To address all issues possible (including breaking changes), run:
2025-11-13 15:52:21.7844 IST [Polaris Coverity Capture] INFO:   npm audit fix --force
2025-11-13 15:52:21.7844 IST [Polaris Coverity Capture] INFO: 
2025-11-13 15:52:21.7844 IST [Polaris Coverity Capture] INFO: Some issues need review, and may require choosing
2025-11-13 15:52:21.7844 IST [Polaris Coverity Capture] INFO: a different dependency.
2025-11-13 15:52:21.7844 IST [Polaris Coverity Capture] INFO: 
2025-11-13 15:52:21.7844 IST [Polaris Coverity Capture] INFO: Run `npm audit` for details.
2025-11-13 15:52:22.0744 IST [Polaris Coverity Capture] INFO: Attempting to detect unconfigured compilers in build
2025-11-13 15:52:22.0811 IST [Polaris Coverity Capture] INFO: |0----------25-----------50----------75---------100|
2025-11-13 15:52:22.1851 IST [Polaris Coverity Capture] INFO: ****************************************************
2025-11-13 15:52:22.2138 IST [Polaris Coverity Capture] WARNING: Recorded 0 C/C++ compilation units (0%) successfully. These compilation units are ready for replay
2025-11-13 15:52:22.2139 IST [Polaris Coverity Capture] WARNING: Recoverable errors were encountered during 1 of these C/C++ compilation units.
2025-11-13 15:52:22.2139 IST [Polaris Coverity Capture] INFO: 
2025-11-13 15:52:22.2139 IST [Polaris Coverity Capture] INFO:  For more details, please look at: 
2025-11-13 15:52:22.2139 IST [Polaris Coverity Capture] INFO:     /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/build-log.txt
2025-11-13 15:52:22.2909 IST [Polaris Coverity Capture] INFO: Executing action Collect Build Metrics
2025-11-13 15:52:22.2912 IST [Polaris Coverity Capture] INFO: Executing action Invalidate capture results
2025-11-13 15:52:22.2913 IST [Polaris Coverity Capture] INFO: Executing action Update uncaptured file timestamps for project "/Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/node_modules/consolidate/Makefile"
2025-11-13 15:52:22.2914 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir list-capture-diagnostics
2025-11-13 15:52:23.3543 IST [Polaris Coverity Capture] INFO: Executing action Emit files using buildless capture: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-internal-capture-files --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --ticker-mode none --append-log --capture-list-file /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/capture-file-list-2947428563 --record-with-source
2025-11-13 15:52:23.3849 IST [Polaris Coverity Capture] INFO: Buildless capture started.
2025-11-13 15:52:23.3993 IST [Polaris Coverity Capture] INFO: Emitting 84 Files.
2025-11-13 15:52:23.5772 IST [Polaris Coverity Capture] INFO: Buildless capture completed.
2025-11-13 15:52:23.5799 IST [Polaris Coverity Capture] INFO: Executing action Delete unwanted TUs: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit @@/Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/delete-unwanted-tus-action-821759241
2025-11-13 15:52:23.5999 IST [Polaris Coverity Capture] INFO: Executing action Action cleanup: Unwanted TUs action cleanup
2025-11-13 15:52:23.6002 IST [Polaris Coverity Capture] INFO: Executing action deleteResidualTUs /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir
2025-11-13 15:52:23.6004 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir list-capture-diagnostics
2025-11-13 15:52:23.6177 IST [Polaris Coverity Capture] INFO: Executing action Invalidate capture results
2025-11-13 15:52:23.6178 IST [Polaris Coverity Capture] INFO: Executing action Invoke cov-run-sigma: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-run-sigma --project-dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir --coverity-config /var/folders/wm/gkd75sk54h57yqd0_j95gp2r0000gn/T/cov-run-sigma-config-151553869/coverity.yaml --sigma-binary-path /Users/madhusud/.blackduck/bridge/tools/sigma/2025.10.0/sigma --enable-telemetry
2025-11-13 15:52:23.6554 IST [Polaris Coverity Capture] INFO: cov-run-sigma version 2025.9.0 on Darwin 24.6.0 arm64
2025-11-13 15:52:23.6554 IST [Polaris Coverity Capture] INFO: Internal version numbers: 477d3c5ddd p-2025.9-push-57
2025-11-13 15:52:23.6554 IST [Polaris Coverity Capture] INFO: 
2025-11-13 15:52:25.3680 IST [Polaris Coverity Capture] INFO: Executing action Action cleanup: Coverity configuration for Sigma
2025-11-13 15:52:26.2850 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir list-capture-diagnostics
2025-11-13 15:52:26.3752 IST [Polaris Coverity Capture] INFO: Capture summary:
2025-11-13 15:52:26.3753 IST [Polaris Coverity Capture] INFO:     SUCCEEDED: 88
2025-11-13 15:52:26.3753 IST [Polaris Coverity Capture] INFO:     INCOMPLETE: 0
2025-11-13 15:52:26.3753 IST [Polaris Coverity Capture] INFO:     FAILED: 0
2025-11-13 15:52:26.3753 IST [Polaris Coverity Capture] INFO:     IGNORED: 3
2025-11-13 15:52:26.3753 IST [Polaris Coverity Capture] INFO:     FILES CAPTURED: 88
2025-11-13 15:52:26.3753 IST [Polaris Coverity Capture] INFO:     LINES OF CODE: 32931
2025-11-13 15:52:26.3784 IST [Polaris Coverity Capture] INFO: Capture phase took 45.982s.
2025-11-13 15:52:26.3785 IST [Polaris Coverity Capture] WARNING: !! SOURCES FOR UNSUPPORTED LANGUAGES WERE DETECTED !!
2025-11-13 15:52:26.3785 IST [Polaris Coverity Capture] WARNING: 
2025-11-13 15:52:26.3785 IST [Polaris Coverity Capture] WARNING: Source files for the following languages were detected, but these languages are not supported on Mac OS ARM:
2025-11-13 15:52:26.3785 IST [Polaris Coverity Capture] WARNING:   * C#
2025-11-13 15:52:26.3785 IST [Polaris Coverity Capture] WARNING: In order to analyze these files, please analyze the project on an operating system and architecture where they are supported.
2025-11-13 15:52:26.4628 IST [Polaris Coverity Capture] INFO: To analyze your project, type '/Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/coverity analyze --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir -o analyze.location=connect'.
2025-11-13 15:52:26.4653 IST [Polaris Coverity Capture] INFO: Coverity Capture completed successfully
2025-11-13 15:52:26.4722 IST [Polaris Coverity Capture] INFO: Provided value for resource 'coverity.completed'
2025-11-13 15:52:26.4723 IST [Polaris Coverity Capture] INFO: Provided value for resource 'coverity.idir.output'
2025-11-13 15:52:26.4728 IST [Polaris Coverity Capture] INFO: Provided value for resource 'polaris.test.sast.tests.sastFull.artifacts.path'
2025-11-13 15:52:26.4731 IST [Polaris Coverity Capture] INFO: Adapter finished
2025-11-13 15:52:26.4752 IST [Bridge CLI] INFO: Starting Adapter: Default Adapter for execution path
2025-11-13 15:52:26.4753 IST [Default Adapter for execution path] INFO: Provided value for resource 'detect.execution.path'
2025-11-13 15:52:26.4753 IST [Default Adapter for execution path] INFO: Adapter finished
2025-11-13 15:52:26.5127 IST [Polaris SCA Package Manager Scan] INFO: Running command /Library/Java/JavaVirtualMachines/jdk-21.jdk/Contents/Home/bin/java -jar /Users/madhusud/.blackduck/bridge/tools/blackduck-detect/10.4.0/detect-10.4.0.jar --detect.cleanup=false --detect.bdio.file.name=scan --detect.detector.search.depth=3 --detect.bdio.output.path=/Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/bdio/blackduck_artifact --detect.output.path=/Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect --detect.tools=DETECTOR --detect.component.location.analysis.enabled=true --blackduck.offline.mode=true --blackduck.offline.mode.force.bdio=true --detect.diagnostic=true
2025-11-13 15:52:27.0000 IST [Polaris SCA Package Manager Scan][main] WARNING: --- Detect-Self-Updater:  Self-Update feature is disabled because of the following reasons:
2025-11-13 15:52:27.0000 IST [Polaris SCA Package Manager Scan][main] WARNING: --- Detect-Self-Updater:  Detect in offline mode is incompatible with the Self-Update feature.
2025-11-13 15:52:27.0000 IST [Polaris SCA Package Manager Scan][main] WARNING: --- Detect-Self-Updater:  Black Duck URL is required for the Self-Update feature.
2025-11-13 15:52:27.2640 IST [Polaris SCA Package Manager Scan] INFO: ______     _            _
2025-11-13 15:52:27.2641 IST [Polaris SCA Package Manager Scan] INFO: |  _  \   | |          | |
2025-11-13 15:52:27.2641 IST [Polaris SCA Package Manager Scan] INFO: | | | |___| |_ ___  ___| |_
2025-11-13 15:52:27.2641 IST [Polaris SCA Package Manager Scan] INFO: | | | / _ \ __/ _ \/ __| __|
2025-11-13 15:52:27.2641 IST [Polaris SCA Package Manager Scan] INFO: | |/ /  __/ ||  __/ (__| |_
2025-11-13 15:52:27.2641 IST [Polaris SCA Package Manager Scan] INFO: |___/ \___|\__\___|\___|\__|
2025-11-13 15:52:27.2641 IST [Polaris SCA Package Manager Scan] INFO: 
2025-11-13 15:52:27.3871 IST [Polaris SCA Package Manager Scan] INFO: 
2025-11-13 15:52:27.3871 IST [Polaris SCA Package Manager Scan] INFO: Detect Version: 10.4.0
2025-11-13 15:52:27.3872 IST [Polaris SCA Package Manager Scan] INFO: 
2025-11-13 15:52:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 15:52:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Current property values:
2025-11-13 15:52:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- --property = value [notes]
2025-11-13 15:52:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ------------------------------------------------------------
2025-11-13 15:52:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- blackduck.offline.mode = true [cmd] 
2025-11-13 15:52:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- blackduck.offline.mode.force.bdio = true [cmd] 
2025-11-13 15:52:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.bdio.file.name = scan [cmd] 
2025-11-13 15:52:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.bdio.output.path = /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/bdio/blackduck_artifact [cmd] 
2025-11-13 15:52:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.cleanup = false [cmd] 
2025-11-13 15:52:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.component.location.analysis.enabled = true [cmd] 
2025-11-13 15:52:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.detector.search.depth = 3 [cmd] 
2025-11-13 15:52:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.diagnostic = true [cmd] 
2025-11-13 15:52:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.excluded.directories = /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge [env] 
2025-11-13 15:52:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.output.path = /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect [cmd] 
2025-11-13 15:52:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.tools = DETECTOR [cmd] 
2025-11-13 15:52:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ------------------------------------------------------------
2025-11-13 15:52:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 15:52:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Detect build date: 2025-04-24
2025-11-13 15:52:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Source directory: /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm
2025-11-13 15:52:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Output directory: /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect
2025-11-13 15:52:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Run directory: /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-10-22-27-347
2025-11-13 15:52:27.4897 IST [Polaris SCA Package Manager Scan] INFO: 
2025-11-13 15:52:27.4897 IST [Polaris SCA Package Manager Scan] INFO: ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
2025-11-13 15:52:27.4898 IST [Polaris SCA Package Manager Scan] INFO: Diagnostic mode on.
2025-11-13 15:52:27.4898 IST [Polaris SCA Package Manager Scan] INFO: A zip file will be created with logs and relevant Detect output files.
2025-11-13 15:52:27.4898 IST [Polaris SCA Package Manager Scan] INFO: It is generally not recommended to leave diagnostic mode on as you must manually clean up the zip.
2025-11-13 15:52:27.4898 IST [Polaris SCA Package Manager Scan] INFO: ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
2025-11-13 15:52:27.4899 IST [Polaris SCA Package Manager Scan] INFO: 
2025-11-13 15:52:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Initializing diagnostic components.
2025-11-13 15:52:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Created report file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-10-22-27-347/reports/search_report.txt
2025-11-13 15:52:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Created report file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-10-22-27-347/reports/search_detailed_report.txt
2025-11-13 15:52:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Created report file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-10-22-27-347/reports/detector_report.txt
2025-11-13 15:52:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Created report file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-10-22-27-347/reports/detector_profile_report.txt
2025-11-13 15:52:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Created report file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-10-22-27-347/reports/code_location_report.txt
2025-11-13 15:52:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Created report file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-10-22-27-347/reports/dependency_counts_report.txt
2025-11-13 15:52:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Created report file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-10-22-27-347/reports/detect_configuration.txt
2025-11-13 15:52:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Attempting to capture sysout.
2025-11-13 15:52:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Writing sysout to file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-10-22-27-347/logs/sysout.txt
2025-11-13 15:52:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Attempting to set 'com.blackduck.integration' logging level.
2025-11-13 15:52:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Attempting to capture additional log messages to files.
2025-11-13 15:52:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Redirected to file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-10-22-27-347/logs/all.txt
2025-11-13 15:52:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Redirected to file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-10-22-27-347/logs/debug.txt
2025-11-13 15:52:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Redirected to file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-10-22-27-347/logs/info.txt
2025-11-13 15:52:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Attempting to restrict console to debug level (additional levels written to files).
2025-11-13 15:52:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Adding additional log listeners to extractions.
2025-11-13 15:52:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Diagnostics is now in control of logging!
2025-11-13 15:52:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Creating configuration diagnostics reports.
2025-11-13 15:52:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Diagnostics system is ready.
2025-11-13 15:52:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 15:52:27.0000 IST [Polaris SCA Package Manager Scan][main] WARNING: --- Correlated Scanning is not available for Rapid/Stateless scan mode or offline scanning. A correlation ID will not be set.
2025-11-13 15:52:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 15:52:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Docker tool will not be run.
2025-11-13 15:52:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 15:52:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Bazel tool will not be run.
2025-11-13 15:52:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 15:52:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Will include the Detectors tool.
2025-11-13 15:52:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Searching for detectors.
2025-11-13 15:52:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Evaluating detectors. This may take a while.
2025-11-13 15:52:28.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ======================================================================================================
2025-11-13 15:52:28.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Detector Report
2025-11-13 15:52:28.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ======================================================================================================
2025-11-13 15:52:28.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 	/Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm (depth 0)
2025-11-13 15:52:28.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 		NPM Package Lock: SUCCESS
2025-11-13 15:52:28.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 			Found file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/package-lock.json
2025-11-13 15:52:28.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 			Found file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/package.json
2025-11-13 15:52:28.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 15:52:28.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Saved file to diagnostics zip: /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/package-lock.json
2025-11-13 15:52:28.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Saved file to diagnostics zip: /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/package.json
2025-11-13 15:52:28.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Detectors actions finished.
2025-11-13 15:52:28.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 15:52:28.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Project name: owasp-nodejs-goat
2025-11-13 15:52:28.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Project version: 1.3.0
2025-11-13 15:52:29.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 15:52:29.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Signature Scanner tool will not be run.
2025-11-13 15:52:29.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 15:52:29.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Vulnerability Impact Analysis tool will not be run.
2025-11-13 15:52:29.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 15:52:29.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- IaC Scanner tool will not be run.
2025-11-13 15:52:29.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 15:52:29.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ##################################################################################################
2025-11-13 15:52:29.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #                                                                                                #
2025-11-13 15:52:29.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  Product Notice                                                                                #
2025-11-13 15:52:29.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  © 2024 Black Duck Software, Inc.                                                              #
2025-11-13 15:52:29.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  This Black Duck Component Locator and all associated documentation are proprietary            #
2025-11-13 15:52:29.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  to Black Duck Software, Inc. and may only be used pursuant to the terms and conditions of a   #
2025-11-13 15:52:29.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  written license agreement with Black Duck Software, Inc. All other use, reproduction,         #
2025-11-13 15:52:29.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  modification, or distribution of the Black Duck Component Locator or the associated           #
2025-11-13 15:52:29.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  documentation is strictly prohibited.                                                         #
2025-11-13 15:52:29.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #                                                                                                #
2025-11-13 15:52:29.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ##################################################################################################
2025-11-13 15:52:29.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Running Component Locator v1.1.12 on /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm
2025-11-13 15:53:34.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Component Location Analysis file saved at: /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-10-22-27-347/scan/components-with-locations.json
2025-11-13 15:53:34.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 15:53:34.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 15:53:34.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 15:53:34.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Creating status file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-10-22-27-347/status/status.json
2025-11-13 15:53:34.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 15:53:34.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Finishing diagnostic mode.
2025-11-13 15:53:34.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Finishing reports.
2025-11-13 15:53:34.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Finishing logging.
2025-11-13 15:53:34.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Finishing executable capture.
2025-11-13 15:53:34.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Finishing file capture.
2025-11-13 15:53:34.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Creating diagnostics zip.
2025-11-13 15:53:34.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Diagnostics zip location: /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/detect-run-2025-11-13-10-22-27-347.zip
2025-11-13 15:53:34.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Diagnostics file created at: /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/detect-run-2025-11-13-10-22-27-347.zip
2025-11-13 15:53:34.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Diagnostic mode has completed.
2025-11-13 15:53:34.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Skipping cleanup, it is disabled.
2025-11-13 15:53:34.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 15:53:34.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 15:53:34.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ======== Detect Result ========
2025-11-13 15:53:34.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 15:53:34.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Component Location Analysis File: /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-10-22-27-347/scan/components-with-locations.json
2025-11-13 15:53:34.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 15:53:34.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ======== Detect Status ========
2025-11-13 15:53:34.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 15:53:34.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- NPM: SUCCESS
2025-11-13 15:53:34.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Overall Status: SUCCESS - Detect exited successfully.
2025-11-13 15:53:34.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 15:53:34.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ===============================
2025-11-13 15:53:34.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 15:53:34.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Detect duration: 00h 01m 07s 332ms
2025-11-13 15:53:34.1946 IST [Polaris SCA Package Manager Scan] INFO: Provided value for resource 'detect.completed'
2025-11-13 15:53:34.1947 IST [Polaris SCA Package Manager Scan] INFO: Provided value for resource 'polaris.test.sca.tests.scaPackage.artifacts.path'
2025-11-13 15:53:34.1950 IST [Polaris SCA Package Manager Scan] INFO: Adapter finished
2025-11-13 15:53:34.2545 IST [Polaris Artifacts Uploader] INFO: uploading artifact for "SAST(sastFull)" assessment with id "b724bbe5-af26-4468-b689-55223ccc5029"
2025-11-13 15:53:34.2550 IST [Polaris Artifacts Uploader] INFO: uploading artifact for "SCA(scaPackage)" assessment with id "52811fce-6884-4f11-8317-aaf523769a8d"
2025-11-13 15:53:35.8678 IST [Polaris Artifacts Uploader] INFO: Uploading artifact /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/blackduck-sca-artifacts.zip for "SCA(scaPackage)" assessment
2025-11-13 15:53:35.9819 IST [Polaris Artifacts Uploader] INFO: Uploading artifact /Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_coverity_capture/idir.zip for "SAST(sastFull)" assessment
2025-11-13 15:53:36.5501 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact:   0%  16384/1761824
2025-11-13 15:53:36.5560 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SCA(scaPackage)" artifact:   6%  16384/235729
2025-11-13 15:53:36.7640 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SCA(scaPackage)" artifact:  34%  81920/235729
2025-11-13 15:53:36.7666 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SCA(scaPackage)" artifact:  62%  147456/235729
2025-11-13 15:53:37.1907 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SCA(scaPackage)" artifact:  90%  212992/235729
2025-11-13 15:53:37.1909 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SCA(scaPackage)" artifact: 100%  235729/235729
2025-11-13 15:53:37.3921 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact:  25%  442368/1761824
2025-11-13 15:53:37.6222 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact:  50%  884736/1761824
2025-11-13 15:53:37.6349 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact:  75%  1327104/1761824
2025-11-13 15:53:37.8801 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact: 100%  1761824/1761824
2025-11-13 15:53:37.8830 IST [Polaris Artifacts Uploader] INFO: successfully uploaded artifact "/Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/blackduck-sca-artifacts.zip"
2025-11-13 15:53:38.4583 IST [Polaris Artifacts Uploader] INFO: successfully resumed "SCA(scaPackage)" assessment with id "52811fce-6884-4f11-8317-aaf523769a8d"
2025-11-13 15:53:38.4920 IST [Polaris Artifacts Uploader] INFO: successfully uploaded artifact "/Users/madhusud/Jenkins_Testing/Nodes/workspace/b_Polaris_Detailed_Workflow_main/nodejs-npm/.bridge/polaris_coverity_capture/idir.zip"
2025-11-13 15:53:38.9824 IST [Polaris Artifacts Uploader] INFO: successfully resumed "SAST(sastFull)" assessment with id "b724bbe5-af26-4468-b689-55223ccc5029"
2025-11-13 15:53:39.0114 IST [Polaris Artifacts Uploader] INFO: Provided value for resource 'polaris.test.sast.tests.sastFull.artifacts.uploadSuccessful'
2025-11-13 15:53:39.0120 IST [Polaris Artifacts Uploader] INFO: Provided value for resource 'polaris.test.sca.tests.scaPackage.artifacts.uploadSuccessful'
2025-11-13 15:53:39.0127 IST [Polaris Artifacts Uploader] INFO: Adapter finished
2025-11-13 15:53:39.1044 IST [Polaris Waiter] INFO: Waiting for test with assessment type "SAST(sastFull)" and id "b724bbe5-af26-4468-b689-55223ccc5029"
2025-11-13 15:53:39.1051 IST [Polaris Waiter] INFO: Waiting for test with assessment type "SCA(scaPackage)" and id "52811fce-6884-4f11-8317-aaf523769a8d"
2025-11-13 15:53:39.8825 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SCA(scaPackage)" and id "52811fce-6884-4f11-8317-aaf523769a8d" is "Waiting for Capture"
2025-11-13 15:53:39.8855 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SAST(sastFull)" and id "b724bbe5-af26-4468-b689-55223ccc5029" is "Waiting for Capture"
2025-11-13 15:53:50.1932 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SAST(sastFull)" and id "b724bbe5-af26-4468-b689-55223ccc5029" is "Queuing"
2025-11-13 15:53:50.1974 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SCA(scaPackage)" and id "52811fce-6884-4f11-8317-aaf523769a8d" is "Queuing"
2025-11-13 15:54:00.4935 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SAST(sastFull)" and id "b724bbe5-af26-4468-b689-55223ccc5029" is "Scanning"
2025-11-13 15:54:00.4947 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SCA(scaPackage)" and id "52811fce-6884-4f11-8317-aaf523769a8d" is "Scanning & Publishing"
2025-11-13 15:54:10.8096 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SAST(sastFull)" and id "b724bbe5-af26-4468-b689-55223ccc5029" is "In Progress"
2025-11-13 15:54:21.0974 IST [Polaris Waiter] INFO: test with assessment type "SCA(scaPackage)" and id "52811fce-6884-4f11-8317-aaf523769a8d" completed successfully
2025-11-13 15:54:21.1111 IST [Polaris Waiter] INFO: test with assessment type "SAST(sastFull)" and id "b724bbe5-af26-4468-b689-55223ccc5029" completed successfully
2025-11-13 15:54:21.1442 IST [Polaris Waiter] INFO: Provided value for resource 'polaris.test.sast.tests.sastFull.completed'
2025-11-13 15:54:21.1444 IST [Polaris Waiter] INFO: Provided value for resource 'polaris.test.sca.tests.scaPackage.completed'
2025-11-13 15:54:21.1448 IST [Polaris Waiter] INFO: Adapter finished
2025-11-13 15:54:21.2426 IST [Polaris Policy Checker] INFO: Checking for policy violations for "SAST(sastFull)" assessment...
2025-11-13 15:54:21.2429 IST [Polaris Policy Checker] INFO: Checking for policy violations for "SCA(scaPackage)" assessment...
2025-11-13 15:54:22.3252 IST [Polaris Policy Checker] INFO: no policies were violated to break the build
2025-11-13 15:54:22.3591 IST [Polaris Policy Checker] INFO: Adapter finished
2025-11-13 15:54:22.4186 IST [Polaris Issues Fetcher] INFO: Fetching issues for "SAST(sastFull)" assessment
2025-11-13 15:54:22.4194 IST [Polaris Issues Fetcher] INFO: Fetching issues for "SCA(scaPackage)" assessment
2025-11-13 15:54:23.3010 IST [Polaris Issues Fetcher] INFO: Successfully fetched issues for assessment type "SAST(sastFull)" with id "b724bbe5-af26-4468-b689-55223ccc5029"
 {
 "critical": 0,
 "high": 2,
 "informational": 0,
 "low": 25,
 "medium": 13
}
2025-11-13 15:54:23.3171 IST [Polaris Issues Fetcher] INFO: Successfully fetched issues for assessment type "SCA(scaPackage)" with id "52811fce-6884-4f11-8317-aaf523769a8d"
 {
 "critical": 6,
 "high": 109,
 "informational": 0,
 "low": 15,
 "medium": 133
}
2025-11-13 15:54:23.3563 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.sast.tests.sastFull.issues.low'
2025-11-13 15:54:23.3567 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.sast.tests.sastFull.issues.medium'
2025-11-13 15:54:23.3571 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.sast.tests.sastFull.issues.critical'
2025-11-13 15:54:23.3574 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.sast.tests.sastFull.issues.informational'
2025-11-13 15:54:23.3578 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.sast.tests.sastFull.issues.high'
2025-11-13 15:54:23.3581 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.sca.tests.scaPackage.issues.low'
2025-11-13 15:54:23.3585 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.sca.tests.scaPackage.issues.critical'
2025-11-13 15:54:23.3588 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.sca.tests.scaPackage.issues.informational'
2025-11-13 15:54:23.3592 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.sca.tests.scaPackage.issues.medium'
2025-11-13 15:54:23.3596 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.sca.tests.scaPackage.issues.high'
2025-11-13 15:54:23.3603 IST [Polaris Issues Fetcher] INFO: Adapter finished
2025-11-13 15:54:24.8265 IST [Polaris SARIF Issues Fetcher] INFO: Fetching issues from Polaris Server...
2025-11-13 15:55:26.4372 IST [Polaris SARIF Issues Fetcher] INFO: Added entry to resource 'polaris.reports.sarif.issues'
2025-11-13 15:55:26.4456 IST [Bridge CLI] INFO: Starting adapters for stage polaris-sarif-generator
2025-11-13 15:55:26.4458 IST [Bridge CLI] INFO: Starting Adapter: Polaris SARIF Generator
2025-11-13 15:55:26.4461 IST [Polaris SARIF Issues Fetcher] INFO: Adapter finished
2025-11-13 15:55:26.5238 IST [Polaris Status Provider] INFO: Results for test "SCA(scaPackage)" with ID "52811fce-6884-4f11-8317-aaf523769a8d" are available at https://poc.polaris.blackduck.com/portfolio/portfolios/edf596d3-b54f-4a6b-9e5c-209f2e526c67/portfolio-items/8a1259ec-ad21-47ce-a755-cb6d96d9f329/projects/77fd4955-2c78-49c2-bab5-680ed8575b99/tests/52811fce-6884-4f11-8317-aaf523769a8d/detected-issues
2025-11-13 15:55:26.5242 IST [Polaris Status Provider] INFO: Results for test "SAST(sastFull)" with ID "b724bbe5-af26-4468-b689-55223ccc5029" are available at https://poc.polaris.blackduck.com/portfolio/portfolios/edf596d3-b54f-4a6b-9e5c-209f2e526c67/portfolio-items/8a1259ec-ad21-47ce-a755-cb6d96d9f329/projects/77fd4955-2c78-49c2-bab5-680ed8575b99/tests/b724bbe5-af26-4468-b689-55223ccc5029/detected-issues
2025-11-13 15:55:26.5242 IST [Polaris Status Provider] INFO: Polaris issues view for project "detailed-example", branch "main" is available at https://poc.polaris.blackduck.com/portfolio/portfolios/edf596d3-b54f-4a6b-9e5c-209f2e526c67/portfolio-items/8a1259ec-ad21-47ce-a755-cb6d96d9f329/projects/77fd4955-2c78-49c2-bab5-680ed8575b99/issues?branchId=c9a05d59-6c9c-4ae1-8661-61d6a38179cb
2025-11-13 15:55:26.5317 IST [Polaris Status Provider] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.summary.url'
2025-11-13 15:55:26.5319 IST [Polaris Status Provider] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.summary.url'
2025-11-13 15:55:26.5320 IST [Polaris Status Provider] INFO: Provided value for resource 'polaris.project.issues.url'
2025-11-13 15:55:26.5323 IST [Polaris Status Provider] INFO: Adapter finished
2025-11-13 15:55:27.7864 IST [Polaris SARIF Generator] INFO: Will create rules with SCA component-version pairs grouped by their related vulnerabilities in the SARIF report. Since "polaris.reports.sarif.groupSCAIssues" is configured to "true"
2025-11-13 15:55:27.7949 IST [Polaris SARIF Generator] INFO: SARIF report created successfully at .blackduck/integrations/polaris/sarif/report.sarif.json
2025-11-13 15:55:27.8272 IST [Polaris SARIF Generator] INFO: Provided value for resource 'polaris.reports.sarif.file.output'
2025-11-13 15:55:27.8277 IST [Polaris SARIF Generator] INFO: Adapter finished
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
Build Number: 3
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