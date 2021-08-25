sulhomeblog
===========

Sample code for articles published on sulhome.com

# ServiceRouting Branch
+ https://github.com/sulhome/sulhomeblog/tree/ServiceRouting
+ https://www.sulhome.com/blog/4/service-versioning-using-wcf-routing

# WCF Versioning
+ It depends on many things such as what changes you are going to make, what platform your clients are built on, what's your change tracking policy, etc.

+ For example if you just want to add a new property to a data contract or a new operation to a service contract it's safe to add it to your current implementation as long as the clients are version tolerant (DataContractSerializer is version tolerant) and it complies with your change tracking policy. However you would better stick to strict versioning strategy which requires creating a new contract and exposing it with a new endpoint in case the changes are more serious.

+ I suggested reading these articles:

  + Versioning Strategies
  + Best Practices: Data Contract Versioning
