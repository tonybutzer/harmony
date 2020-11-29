# Glossary

---
- **Agency Problem:**
> The **agency problem** is a conflict of interest inherent in any relationship where one party is expected to act in another's best interests. In corporate finance, the agency problem usually refers to a conflict of interest between a company's management and the company's stockholders.  ['Windows OS', 'Kubernetes?']

---
- **COG**
> What are Cloud Optimized GeoTIFFs (COGs)?

> A **Cloud Optimized GeoTIFF (COG)** is a GeoTIFF file with an internal organization that enables more efficient workflows in the cloud environment.  It does this by leveraging the ability of clients issuing HTTP GET range requests to ask for just the parts of a file they need.
*Geek Hint:* Use rio info and gdalinfo to see the innards of a COG and the overviews associated with a COG.
For more info talk to THE GOOGLE.

---
- **Data Lake**

---
- **DataOps**
> DataOps is an automated, process-oriented methodology, used by analytic and data teams, to improve the quality and reduce the cycle time of data analytics. While DataOps began as a set of best practices, it has now matured to become a new and independent approach to data analytics. - Cassandra Ladino USGS ACIO has experience in DataOps
---
> What is DataOps?

> DataOps is a collection of technical practices, workflows, cultural norms, and architectural patterns that enable:

    - Rapid innovation and experimentation, delivering new insights to customers with increasing velocity

    - Extremely high quality and very low error rates

    - Collaboration across complex arrays of people, technology, and environments

    - Clear measurement, monitoring and transparency of results


---
- **Dark Repository**



- **DevOps**
> DevOps Model Defined

---
> DevOps is the combination of cultural philosophies, practices, and tools that increases an organization’s ability to deliver applications and services at high velocity: evolving and improving products at a faster pace than organizations using traditional software development and infrastructure management processes. This speed enables organizations to better serve their customers and compete more effectively in the market. [https://aws.amazon.com/devops/what-is-devops/](https://aws.amazon.com/devops/what-is-devops/)



- **Imposter Syndrome:**
> **Imposter syndrome** can be defined as a collection of feelings of inadequacy that persist despite evident success. 'Imposters' suffer from chronic self-doubt and a sense of intellectual fraudulence that override any feelings of success or external proof of their competence


---
- **Jupyter (Notebook and Hub)**

---
- **PANGEO**



---
- **STAC**
> STAC is a standardized way to expose collections of spatial temporal data. ... It can be used for external access to your holdings, exposing your information to search engines and to a growing ecosystem of tools.
---
> "So STAC itself has no aim to provide one single index, but to encourage the basic unit of information from which a variety of indexes can be built. For STAC that basic unit is the actual geospatial asset and a JSON description of the core fields. This mirrors the design of the web as a whole: html pages are the basic unit of information, and companies like Google build the global search index. Creating a great geospatial search index is left to others to innovate on, but the STAC spec aims to encourage software implementations and data providers to expose their holdings in a way that everyone can understand." - Chris Holmes
---
> Chris Holmes Product Architect @ Planet, Board Member @ Open Geospatial Consortium, Technical Fellow @ Radiant.Earth -- Chris's medium articles contain well-written descriptuions of these cloud optimized ecosystems that can be exploited to simplify science.

---
- **terraform**

> Terraform is an open-source infrastructure as code software tool created by HashiCorp. Users define and provision data center infrastructure using a declarative configuration language known as HashiCorp Configuration Language, or optionally JSON. Terraform manages external resources with "providers"

> **terraform** creates infrastructure out of thin air - **teraform** allows tony to feel like Bob Ross painting infrastucture "lets have a nice litte server here ... next to our little network here and a lovely little data bucket over there."
```
$ scp bob_ross.PNG ubuntu@`resolv hweb`:.
```
![](./Assets/bob_ross.PNG)
