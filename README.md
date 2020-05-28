# Hanh ApplicationProcess Project
Sln: Hanh.ApplicationProcess.May2020

The following projects:
Hahn.ApplicatonProcess.May2020.Data - netstandard2.1 
Hahn.ApplicatonProcess.May2020.Domain - netstandard2.1 
Hahn.ApplicatonProcess.May2020.Web - netcoreapp3.1

The web project is self-hosted using Krestel. Once loaded up in VS 2019 (16.6), please do Restore NUGet Packages, didn't include them as per instructions.

These are the following endpoints:

POST: /Applicat/AddApplicant
GET: /Applicant/GetApplicants and /Applicant/GetApplicant/{id}
PUT: /Applicant/UpdateApplicant
DELETE: /Applicant/Delete/{id}
Also, created pages for this so you can play around. Once the web is up, you'll be able to see as default view a list of 6 existing applicants, which is added InMemory. There you can Add, Edit, Delete, and, also a page where it allows you to post json raw object to add an applicant.

Fluent Validation has been implemented as well on the applicant object class per the requirement. Swagger Endpoint can be accessed via {localhost}/swagger/v1/swagger.json Serilog RollingFile is defaulted to C:\logs\log-{Date}.txt

Pending Implementation are the following:

i8Next
json localized string
country validation
Aurelia
and few little details
