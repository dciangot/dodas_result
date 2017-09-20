# **Real Workflow: Long test with small cluster of 3 WNs and reduced input statistics**

* **D meson invariant mass reconstruction with Kpipi decays**

**~4days running time, no issues recorded on WNs for the whole duration**

![](https://lh4.googleusercontent.com/7t9BdmhUnT2QL8HuzDVpPi9a_JDWyCZyx3DZa92gWxdNNMltv2jgq3KNwNwiR1zvqngOmrNZ33MdqGTfcZ9dgdR6PD-lWaGnQ7q1TwhOPoZZvaY32qGhRY3w9vvL805p7VqkjPH_ "Screenshot from 2017-08-29 13-19-50.png")**a - number of jobs running on 1 slave;**

**running dockers cpu usage on the same slave;**

![](https://lh5.googleusercontent.com/5f0DIWR8LxYLrwIJz6JeSeB6d8lvdu3btKjBDF0jy6cI7zMalUfc0t-frPChqwD2LdccHaKbonW4nSgCzEw89V8JfE8WtrQrAcdU7VSwtBIcWLw81fhqVOWLDpsv5YCHWRxJsehM "Screenshot from 2017-08-29 13-20-03.png")**b - slave normalized load \(1min\) by process. cmsRun is in green**

**slave memory usage by process**

![](https://lh6.googleusercontent.com/54OMICu2rhQZcwpqe4b8rkjgRq8v1_mhBBMtRTkVI0AX20K-iYUptteV5QPAMp0snCIq1p8CYK7tyj1-kpslTw5UhkI0BuKqp3HEzVU26dWlXToYPfwr1Qts6WhG0pHRhJLvulMj "Screenshot from 2017-08-29 13-20-15.png")**c - slave free disk space**

  


![](https://lh3.googleusercontent.com/dMpfIDbrcYMunzw1bUA2-h_xS7e9HfBt9kXP9nxPJLYO378-J1Dn67W0m8pTM6TIekV8Vioi21KHHln57L-Aq3a_onqlK9W-nUzbtosf9ZOfqBOCSdcPaMwx6UugvCDA90b2J9J2)

![](https://lh6.googleusercontent.com/9Tj5rZo6eNzojpKhcyoYC1XoyC4hXpB2sRPIvoZBcHMhKGFMvPHeDYB6EQ0jsZp4-JdpYknkrOuh1hd5c-_SNWxwjaQUokgRPBtV_fBdZ8LeABICAS4aCE485pwQVaOrgvhQ0gBa "Dmass\_alldata\_Diego.png")



**INPUT DATASET = /ZeroBias/Run2016C-23Sep2016-v1/AOD**

**DAS link =**[**https://cmsweb.cern.ch/das/request?input=site%20dataset%3D/ZeroBias/Run2016C-23Sep2016-v1/AOD&instance=prod/global&idx=0&limit=10**](https://cmsweb.cern.ch/das/request?input=site%20dataset%3D/ZeroBias/Run2016C-23Sep2016-v1/AOD&instance=prod/global&idx=0&limit=10)

**  
**

[**http://dashb-cms-job.cern.ch/dashboard/templates/task-analysis/\#user=Valentina+Mariani&refresh=0&table=Jobs&p=1&records=25&sorting%5B%5D=3&sorting%5B%5D=desc&activemenu=1&status=&site=&tid=170728\_151922%3Avmariani\_crab\_Dp\_ZB16runC\_testDiegoi\_voms0809**](http://dashb-cms-job.cern.ch/dashboard/templates/task-analysis/#user=Valentina+Mariani&refresh=0&table=Jobs&p=1&records=25&sorting%5B%5D=3&sorting%5B%5D=desc&activemenu=1&status=&site=&tid=170728_151922%3Avmariani_crab_Dp_ZB16runC_testDiegoi_voms0809)

**  
**

**Jobs status: failed 27.3% \(18/66\)**

**finished 72.7% \(48/66\)**

**  
**

* **15 job falliti perche stati troppo in idle: atteso per via delle poche slot**

* **2 job per problemi ad aprire l’input file: niente a che fare con il deploy, ma piuttosto con problemi transienti del source site/xrootd**

* **1 job fallito per stageout in temp area: strano, probabilmente network problem temporaneo**

**  
**

**  
**

**No publication information \(publication has been disabled in the CRAB configuration file\)**

**  
**

**Error Summary:**

**  
**

**15 jobs failed with exit code 50665:**

**  
**

**15 jobs failed with following error message: \(for example, job 1\)**

**  
**

**Not retrying job due to excessive idle time \(job automatically killed on the grid scheduler\)**

**  
**

**2 jobs failed with exit code 8020:**

**  
**

**1 jobs failed with following error message: \(for example, job 57\)**

**  
**

**CmsRunFailure**

**CMSSW error message follows.**

**Fatal Exception**

**An exception of category 'FileOpenError' occurred while**

**\[0\] Calling InputSource::readFile\_**

**\[1\] Calling RootFileSequenceBase::initTheFile\(\)**

**\[2\] Calling StorageFactory::open\(\)**

**\[3\] Calling XrdFile::open\(\)**

**Exception Message:**

**Failed to open the file 'root://xrootd-cms.infn.it:1194//store/data/Run2016C/ZeroBias/AOD/23Sep2016-v1/90000/4A1167C9-A982-E611-A525-A0000420FE80.root'**

**Additional Info:**

**\[a\] Input file root://xrootd-cms.infn.it:1194//store/data/Run2016C/ZeroBias/AOD/23Sep2016-v1/90000/4A1167C9-A982-E611-A525-A0000420FE80.root could not be opened.**

**\[b\] XrdCl::File::Open\(name='root://xrootd-cms.infn.it:1194//store/data/Run2016C/ZeroBias/AOD/23Sep2016-v1/90000/4A1167C9-A982-E611-A525-A0000420FE80.root', flags=0x10, permissions=0660\) =&gt; error '\[ERROR\] Server responded with an error: \[3011\] No servers are available to read the file.**

**' \(errno=3011, code=400\). No additional data servers were found.**

**\[c\] Last URL tried: root://xrootd-cms.infn.it:1194//store/data/Run2016C/ZeroBias/AOD/23Sep2016-v1/90000/4A1167C9-A982-E611-A525-A0000420FE80.root?tried=**

**\[d\] Problematic data server: xrootd-cms.infn.it:1194**

**\[e\] Disabled source: xrootd-cms.infn.it:1194**

**  
**

**1 jobs failed with following error message: \(for example, job 54\)**

**  
**

**CmsRunFailure**

**CMSSW error message follows.**

**Fatal Exception**

**An exception of category 'FileOpenError' occurred while**

**\[0\] Calling InputSource::readFile\_**

**\[1\] Calling RootFileSequenceBase::initTheFile\(\)**

**\[2\] Calling StorageFactory::open\(\)**

**\[3\] Calling XrdFile::open\(\)**

**Exception Message:**

**Failed to open the file 'root://xrootd-cms.infn.it:1194//store/data/Run2016C/ZeroBias/AOD/23Sep2016-v1/90000/B085A583-1C83-E611-BDE9-A0000420FE80.root'**

**Additional Info:**

**\[a\] Input file root://xrootd-cms.infn.it:1194//store/data/Run2016C/ZeroBias/AOD/23Sep2016-v1/90000/B085A583-1C83-E611-BDE9-A0000420FE80.root could not be opened.**

**\[b\] XrdCl::File::Open\(name='root://xrootd-cms.infn.it:1194//store/data/Run2016C/ZeroBias/AOD/23Sep2016-v1/90000/B085A583-1C83-E611-BDE9-A0000420FE80.root', flags=0x10, permissions=0660\) =&gt; error '\[ERROR\] Server responded with an error: \[3010\] Unable to give access - user access restricted - unauthorized identity used ; Permission denied**

**' \(errno=3010, code=400\). No additional data servers were found.**

**\[c\] Last URL tried: root://eoscms.cern.ch:1094//store/data/Run2016C/ZeroBias/AOD/23Sep2016-v1/90000/B085A583-1C83-E611-BDE9-A0000420FE80.root?tried=+1313xrootd.ba.infn.it,**

**\[d\] Problematic data server: eoscms.cern.ch:1094**

**\[e\] Disabled source: eoscms.cern.ch:1094**

**  
**

**1 jobs failed with exit code 60318:**

**  
**

**1 jobs failed with following error message: \(for example, job 56\)**

**  
**

**CmsCpFailure**

**cmscp error message follows.**

**ERROR: Unhandled exception when performing stageout.**

**Traceback \(most recent call last\):**

**File "cmscp.py", line 1405, in main**

**is\_log = False, inject = transfer\_outputs\)**

**File "cmscp.py", line 407, in perform\_stageout**

**source\_site, is\_log, inject\)**

**File "cmscp.py", line 481, in perform\_local\_stageout**

**if stageout\_info\['StageOutReport'\]:**

**TypeError: 'NoneType' object has no attribute '\_\_getitem\_\_'**

**  
**

**Have a look at https://twiki.cern.ch/twiki/bin/viewauth/CMSPublic/JobExitCodes for a description of the exit codes.**

**Log file is /afs/cern.ch/work/d/dciangot/dir\_CMSSW/CMSSW\_7\_0\_5/src/MNTriggerStudies/MNTriggerAna/test/CSA14/crab\_debug/crab\_Dp\_ZB16runC\_testDiegoi\_voms0809/crab.log**

  




