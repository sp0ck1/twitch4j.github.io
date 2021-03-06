---
title: Teams - Get By Name
layout: docs
weight : 71
menu: 
  docs:
    parent: API - Kraken
---

# Get Team by Name

## Description

Gets a specified team object.

## Method Definition

```java
@RequestLine("GET /teams/{name}")
HystrixCommand<KrakenTeam> getTeamByName(
	@Param("name") String name
);
```

*Required Parameters (one of)*

| Name          | Type      | Description  |
| ------------- |:---------:| -----------------:|
| name | string | Name of the team |

*Optional Parameters*

None

## Code-Snippets

### get team by name

{{<codeblocks>}}
{{<code Java>}}
```java
KrakenTeam result = twitchClient.getKraken().getTeamByName("staff").execute();
System.out.println(result.getDisplayName());
```
{{</code>}}
{{<code Groovy>}}
```groovy
def result = twitchClient.kraken.getTeamByName("staff").execute();
System.out.println result.displayName
```
{{</code>}}
{{<code Kotlin>}}
```kotlin
val result = twitchClient.kraken.getTeamByName("staff").execute();
println(result.displayName)
```
{{</code>}}
{{</codeblocks>}}
