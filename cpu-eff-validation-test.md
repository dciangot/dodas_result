# CPU efficiency: CPU time/Run time

Data available in FJR. WMArchive and condor job monitoring is already collecting it, but only for production schedds.

wmarchive -&gt; data.payload.performance.cpu.TotalJobCPU/data.payload.performance.cpu.TotalJobTime  : [http://bit.ly/2wnLWW2](http://bit.ly/2wnLWW2)

condor monitoring -&gt; data.CpuEff: [http://bit.ly/2x1JaoX](http://bit.ly/2x1JaoX)



Some CMS studies refs follow:

![](/assets/cpu_eff.png)![](/assets/cpu_eff2.png)![](/assets/cpu_eff3.png)[https://indico.cern.ch/event/662150/contributions/2703879/attachments/1515249/2364396/Repor\_29\_8\_2017.pdf](https://indico.cern.ch/event/662150/contributions/2703879/attachments/1515249/2364396/Repor_29_8_2017.pdf)

[https://indico.cern.ch/event/656544/contributions/2712028/attachments/1523549/2381779/cms\_lhcc\_wlcg\_Sept\_2017\_-\_CPU\_efficiency.pdf](https://indico.cern.ch/event/656544/contributions/2712028/attachments/1523549/2381779/cms_lhcc_wlcg_Sept_2017_-_CPU_efficiency.pdf)

# Validation test on MC \(FNAL\)

A rough estimation of the overall efficiency is the CPU usage of WN dockers as will be shown below.

CPU usage: % of cpu cycles used/availables

# Avg efficiency ~5% for network waiting ![](/assets/otc_validationSlow.png)

# Validation test on nearer data \(T2\_DE\)![](/assets/otc_validation_fast.png)Avg efficiency ~50%

# 



