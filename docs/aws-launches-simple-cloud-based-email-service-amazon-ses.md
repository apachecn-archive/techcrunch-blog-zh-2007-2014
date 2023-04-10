# AWS 推出简单的批量电子邮件服务 Amazon SES 

> 原文：<https://web.archive.org/web/http://techcrunch.com/2011/01/25/aws-launches-simple-cloud-based-email-service-amazon-ses/>

# AWS 推出简单的批量电子邮件服务 Amazon SES

![](img/52cd982c9abb9beb02767df82dc647cb.png)

[亚马逊网络服务](https://web.archive.org/web/20230203032641/http://www.crunchbase.com/product/amazon-web-services)，Amazon.com 的云计算业务[已经](https://web.archive.org/web/20230203032641/http://www.crunchbase.com/company/amazon)[宣布](https://web.archive.org/web/20230203032641/http://www.businesswire.com/news/home/20110125005939/en/Amazon-Web-Services-Launches-Amazon-Simple-Email)一项新的批量电子邮件服务，称为亚马逊简单电子邮件服务(Amazon SES)。这项基于云的服务面向的是那些不想开发内部电子邮件产品，而是希望调用强大的服务来发送大量电子邮件的开发者和企业。

使用亚马逊 SES 的优势在于它可以与其他 AWS 集成，如托管服务 EC2、亚马逊 S3 等。电子邮件服务是免费的，但亚马逊将根据发送的电子邮件数量和数据传输量收费。亚马逊 SES 的定价是每发送 1000 封电子邮件收取 0.10 美元。此外，客户每天可以免费发送 2，000 封电子邮件，如果这些电子邮件来自亚马逊 EC2 或最近推出的 [AWS Elastic Beanstalk](https://web.archive.org/web/20230203032641/https://techcrunch.com/2011/01/19/amazon-web-services-introduces-elastic-beanstalk-for-easier-app-deployment/) (如果客户超过 AWS 每月免费带宽限额，可能仍会收取数据传输费)。

Amazon SES 使用内容过滤技术来扫描企业的外发电子邮件，以帮助确保内容符合 ISP 标准。然后，该电子邮件要么排队等待发送，要么被路由回发件人以便采取纠正措施。

为了帮助企业提高与客户的电子邮件通信质量，亚马逊 ses 提供了一个内置的反馈循环，其中包括退回通知、失败和成功的递送尝试以及垃圾邮件投诉。