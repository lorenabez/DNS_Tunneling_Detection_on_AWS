# DNS_Tunneling_Detection_on_AWS
Describes an architecture for DNS Tunneling detection at AWS cloud envirement, using ELK.

1. Modules for collecting DNS logs:
  - from AWS VPC flows -> Filebeat (ELK beat)
  - from AWS Route 53 flows -> Filebeat (ELK beat)
  - from DNS resolver  (EC2 instance) on private subnetwork -> Packetbeat (ELK beat)
2. Machine Learning Model:
  - Features analysis and extraction for Machine Learning (ML) jobs;
  - Definition of relevant influencer fields and detectors;
  - ML model for anomaly detection -> Population Analysis Elastic ML Model
3. DNS tunneling tools tests:
  - Iodine
  - Dnscat2
  - DNSExfiltrator
  - DNSStager
  - Flighsim
5. Experiments Results and accurancy

This project and respective improvemments were published on:

English -> "A security model for DNS tunnel detection on cloud platform" https://ieeexplore.ieee.org/abstract/document/9969715

Portuguese -> "IDENTIFICAÇÃO DE TÚNEIS DNS EM NUVEM COMPUTACIONAL USANDO DETECÇÃO DE ANOMALIAS" https://ciaca-conf.org/wp-content/uploads/2022/11/4_CIACA2022_PT_F_068.pdf
