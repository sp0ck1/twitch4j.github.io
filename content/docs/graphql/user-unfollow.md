---
title: User - Unfollow
layout: docs
weight: 21
menu: 
  docs:
    parent: GraphQL
---

# User - Unfollow

## Description

Unfollow a user on twitch.

## Method Definition

*Required Parameters*

| Name          | Type      | Description  |
| ------------- |:---------:| -----------------:|
| authToken | string | User Auth Token |
| targetUserId | number | Target User Id |

*Optional Parameters*

None

## Code-Snippets

### unfollow a user

{{<codeblocks>}}
{{<code Java>}}
```java
twitchClient.getGraphQL().unfollowUser(credential, 24943033l).execute();
```
{{</code>}}
{{<code Groovy>}}
```groovy
twitchClient.graphQL.unfollowUser(credential, 24943033l).execute()
```
{{</code>}}
{{<code Kotlin>}}
```kotlin
twitchClient.graphQL.unfollowUser(credential, 24943033l).execute()
```
{{</code>}}
{{</codeblocks>}}
