# DNS_Tunneling_Detection_on_AWS
Describes an architecture for DNS Tunneling detection at AWS cloud envirement, using ELK.

1. Modules for collecting DNS logs:
  - from AWS VPC flows -> Filebeat (ELK beat)
  - from AWS Route 53 flows -> Filebeat (ELK beat)
  - from DNS resolver  (EC2 instance) on private subnetwork -> Packetbeat (ELK beat)
2. Machine Learning Model:
  - Features analysis and extraction for Machine Learning (ML) jobs;
  - definition of relevant influencer fields and detectors;
  - ML model for anomaly detection -> Population Analysis Elastic ML Model
3. DNS tunneling tools tests:
  - Iodine
  - Dnscat2
  - DNSExfiltrator
5. Experiments Results and accurancy
