Training Reporting
==================

Generate a benchmark reports after running the mila's training benchmarks.


```bash
$ mlbench-report --reports $BASE/ --name fast   --gpu-model RTX
                             target         result           sd       sd%      diff
bench                                                                              
atari                          5.41       7.424253     0.055735  0.007507  0.372320
cart                        2000.00    2195.248475     6.457116  0.002941  0.097624
convnet                      178.76     175.973774     0.191682  0.001089 -0.015586
convnet_distributed          276.10     756.841070    60.333975  0.079718  1.741185
convnet_distributed_fp16     330.41     785.470579    43.330802  0.055165  1.377260
convnet_fp16                 262.56     329.347550     0.770485  0.002339  0.254371
dcgan_all                    139.29     274.608760     1.361280  0.004957  0.971489
dcgan                        115.52     147.794385     0.632454  0.004279  0.279384
fast_style                   156.75     146.285007     0.218744  0.001495 -0.066762
loader                      1200.00    1188.224303    62.070805  0.052238 -0.009813
recom                      20650.19   20802.705368   103.476919  0.004974  0.007386
reso                         138.34     178.694817     0.920870  0.005153  0.291708
ssd                           59.96      49.263719     0.203476  0.004130 -0.178390
toy_lstm                       2.65       1.254635     0.007228  0.005761 -0.526553
toy_reg                   368820.18  215482.487073  3745.776792  0.017383 -0.415752
translator                   223.47     212.040509     0.443492  0.002092 -0.051146
vae                         7972.69    5931.232565    26.450238  0.004459 -0.256056
wlm                         1440.87    1365.497700     2.910483  0.002131 -0.052310
wlmfp16                     3793.37    4649.460342    18.698980  0.004022  0.225681
--

Statistics               |     Value | Pass |
-------------------------|-----------|------|
Bench Passes             :           | True
Deviation Quantile (80%) : +1.1458 % | True |
Performance              : +0.2129 % | True 
--
```

