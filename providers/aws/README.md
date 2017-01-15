Bootstrapping Apache Ambari clusters on AWS
===========================================

Usage
-----

- Open your [AWS CloudFormation
  Console](https://console.aws.amazon.com/cloudformation/home)
- Select the template you wish to use from [./generated/](./generated/)
  - Note: there are 2 versions of each template. You want 'NAME.template.json'
- Provide the file by upload or the 'raw' URL from GitHub.
- CloudFormation will prompt with parameters for your CloudFormation Stack
  - You must select a KeyName.
  - All other fields will work as is and have explanations on screen.

What
----

The current template will:

- Provision a VPC & all requirements
- Provision nodes
- Handle Apache Ambari & HDP requirements
- Install & configure ambari-agent/server using [ambari-bootstrap](../../)

How
---


- The template files were generated with
  [troposphere](https://github.com/cloudtools/troposphere).
- It's currently one big python file, but I plan to split into separate files to
  make generating different versions of templates easier

Known Issues
------------

https://github.com/Vikas2806/HDP-2.5-IOT/ambari-bootstrap/issues

Contacts
--------

- http://github.com/Vikas2806/HDP-2.5-IOT/ambari-bootstrap/
- Vikas Christie: @Vikas2806
