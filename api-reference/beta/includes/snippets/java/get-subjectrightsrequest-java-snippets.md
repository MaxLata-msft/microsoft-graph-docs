---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SubjectRightsRequest subjectRightsRequest = graphClient.privacy().subjectRightsRequests("{subjectRightsRequestId}")
	.buildRequest()
	.get();

```