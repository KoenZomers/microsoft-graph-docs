---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDriveItemDeltaCollectionPage delta = graphClient.me().drive().root()
	.delta("1230919asd190410jlka")
	.buildRequest()
	.get();

```