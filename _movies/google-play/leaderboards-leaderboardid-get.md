---
swagger: "2.0"
info:
  title: Google Play Game Services
  description: The API for Google Play Game Services.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /games/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /leaderboards/{leaderboardId}:
    get:
      summary: Get Leader Board
      description: Retrieves the metadata of the leaderboard with the given ID
      operationId: games.leaderboards.get
      parameters:
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      - in: query
        name: language
        description: The preferred language to use for strings returned by this method
      - in: path
        name: leaderboardId
        description: The ID of the leaderboard
      responses:
        200:
          description: OK
      tags:
      - leader board
definitions:
  AchievementDefinition:
    properties:
      achievementType:
        description: This is a default description.
        type: put
      description:
        description: This is a default description.
        type: put
      experiencePoints:
        description: This is a default description.
        type: put
      formattedTotalSteps:
        description: This is a default description.
        type: put
      id:
        description: This is a default description.
        type: put
      initialState:
        description: This is a default description.
        type: put
      isRevealedIconUrlDefault:
        description: This is a default description.
        type: put
      isUnlockedIconUrlDefault:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      name:
        description: This is a default description.
        type: put
  AchievementDefinitionsListResponse:
    properties:
      items:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      nextPageToken:
        description: This is a default description.
        type: put
  AchievementIncrementResponse:
    properties:
      currentSteps:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      newlyUnlocked:
        description: This is a default description.
        type: put
  AchievementRevealResponse:
    properties:
      currentState:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
  AchievementSetStepsAtLeastResponse:
    properties:
      currentSteps:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      newlyUnlocked:
        description: This is a default description.
        type: put
  AchievementUnlockResponse:
    properties:
      kind:
        description: This is a default description.
        type: put
      newlyUnlocked:
        description: This is a default description.
        type: put
  AchievementUpdateMultipleRequest:
    properties:
      kind:
        description: This is a default description.
        type: put
      updates:
        description: This is a default description.
        type: put
  AchievementUpdateMultipleResponse:
    properties:
      kind:
        description: This is a default description.
        type: put
      updatedAchievements:
        description: This is a default description.
        type: put
  AchievementUpdateRequest:
    properties:
      achievementId:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      updateType:
        description: This is a default description.
        type: put
  AchievementUpdateResponse:
    properties:
      achievementId:
        description: This is a default description.
        type: put
      currentState:
        description: This is a default description.
        type: put
      currentSteps:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      newlyUnlocked:
        description: This is a default description.
        type: put
      updateOccurred:
        description: This is a default description.
        type: put
  AggregateStats:
    properties:
      count:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      max:
        description: This is a default description.
        type: put
      min:
        description: This is a default description.
        type: put
      sum:
        description: This is a default description.
        type: put
  AnonymousPlayer:
    properties:
      avatarImageUrl:
        description: This is a default description.
        type: put
      displayName:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
  Application:
    properties:
      achievement_count:
        description: This is a default description.
        type: put
      assets:
        description: This is a default description.
        type: put
      author:
        description: This is a default description.
        type: put
      description:
        description: This is a default description.
        type: put
      enabledFeatures:
        description: This is a default description.
        type: put
      id:
        description: This is a default description.
        type: put
      instances:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      lastUpdatedTimestamp:
        description: This is a default description.
        type: put
      leaderboard_count:
        description: This is a default description.
        type: put
  ApplicationCategory:
    properties:
      kind:
        description: This is a default description.
        type: put
      primary:
        description: This is a default description.
        type: put
      secondary:
        description: This is a default description.
        type: put
  ApplicationVerifyResponse:
    properties:
      alternate_player_id:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      player_id:
        description: This is a default description.
        type: put
  Category:
    properties:
      category:
        description: This is a default description.
        type: put
      experiencePoints:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
  CategoryListResponse:
    properties:
      items:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      nextPageToken:
        description: This is a default description.
        type: put
  EventBatchRecordFailure:
    properties:
      failureCause:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
  EventChild:
    properties:
      childId:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
  EventDefinition:
    properties:
      childEvents:
        description: This is a default description.
        type: put
      description:
        description: This is a default description.
        type: put
      displayName:
        description: This is a default description.
        type: put
      id:
        description: This is a default description.
        type: put
      imageUrl:
        description: This is a default description.
        type: put
      isDefaultImageUrl:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      visibility:
        description: This is a default description.
        type: put
  EventDefinitionListResponse:
    properties:
      items:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      nextPageToken:
        description: This is a default description.
        type: put
  EventPeriodRange:
    properties:
      kind:
        description: This is a default description.
        type: put
      periodEndMillis:
        description: This is a default description.
        type: put
      periodStartMillis:
        description: This is a default description.
        type: put
  EventPeriodUpdate:
    properties:
      kind:
        description: This is a default description.
        type: put
      updates:
        description: This is a default description.
        type: put
  EventRecordFailure:
    properties:
      eventId:
        description: This is a default description.
        type: put
      failureCause:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
  EventRecordRequest:
    properties:
      currentTimeMillis:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      requestId:
        description: This is a default description.
        type: put
      timePeriods:
        description: This is a default description.
        type: put
  EventUpdateRequest:
    properties:
      definitionId:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      updateCount:
        description: This is a default description.
        type: put
  EventUpdateResponse:
    properties:
      batchFailures:
        description: This is a default description.
        type: put
      eventFailures:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      playerEvents:
        description: This is a default description.
        type: put
  GamesAchievementIncrement:
    properties:
      kind:
        description: This is a default description.
        type: put
      requestId:
        description: This is a default description.
        type: put
      steps:
        description: This is a default description.
        type: put
  GamesAchievementSetStepsAtLeast:
    properties:
      kind:
        description: This is a default description.
        type: put
      steps:
        description: This is a default description.
        type: put
  ImageAsset:
    properties:
      height:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      name:
        description: This is a default description.
        type: put
      url:
        description: This is a default description.
        type: put
      width:
        description: This is a default description.
        type: put
  Instance:
    properties:
      acquisitionUri:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      name:
        description: This is a default description.
        type: put
      platformType:
        description: This is a default description.
        type: put
      realtimePlay:
        description: This is a default description.
        type: put
      turnBasedPlay:
        description: This is a default description.
        type: put
  InstanceAndroidDetails:
    properties:
      enablePiracyCheck:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      packageName:
        description: This is a default description.
        type: put
      preferred:
        description: This is a default description.
        type: put
  InstanceIosDetails:
    properties:
      bundleIdentifier:
        description: This is a default description.
        type: put
      itunesAppId:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      preferredForIpad:
        description: This is a default description.
        type: put
      preferredForIphone:
        description: This is a default description.
        type: put
      supportIpad:
        description: This is a default description.
        type: put
      supportIphone:
        description: This is a default description.
        type: put
  InstanceWebDetails:
    properties:
      kind:
        description: This is a default description.
        type: put
      launchUrl:
        description: This is a default description.
        type: put
      preferred:
        description: This is a default description.
        type: put
  Leaderboard:
    properties:
      iconUrl:
        description: This is a default description.
        type: put
      id:
        description: This is a default description.
        type: put
      isIconUrlDefault:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      name:
        description: This is a default description.
        type: put
      order:
        description: This is a default description.
        type: put
  LeaderboardEntry:
    properties:
      formattedScore:
        description: This is a default description.
        type: put
      formattedScoreRank:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      scoreRank:
        description: This is a default description.
        type: put
      scoreTag:
        description: This is a default description.
        type: put
      scoreValue:
        description: This is a default description.
        type: put
      timeSpan:
        description: This is a default description.
        type: put
      writeTimestampMillis:
        description: This is a default description.
        type: put
  LeaderboardListResponse:
    properties:
      items:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      nextPageToken:
        description: This is a default description.
        type: put
  LeaderboardScoreRank:
    properties:
      formattedNumScores:
        description: This is a default description.
        type: put
      formattedRank:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      numScores:
        description: This is a default description.
        type: put
      rank:
        description: This is a default description.
        type: put
  LeaderboardScores:
    properties:
      items:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      nextPageToken:
        description: This is a default description.
        type: put
      numScores:
        description: This is a default description.
        type: put
      prevPageToken:
        description: This is a default description.
        type: put
  MetagameConfig:
    properties:
      currentVersion:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      playerLevels:
        description: This is a default description.
        type: put
  NetworkDiagnostics:
    properties:
      androidNetworkSubtype:
        description: This is a default description.
        type: put
      androidNetworkType:
        description: This is a default description.
        type: put
      iosNetworkType:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      networkOperatorCode:
        description: This is a default description.
        type: put
      networkOperatorName:
        description: This is a default description.
        type: put
      registrationLatencyMillis:
        description: This is a default description.
        type: put
  ParticipantResult:
    properties:
      kind:
        description: This is a default description.
        type: put
      participantId:
        description: This is a default description.
        type: put
      placing:
        description: This is a default description.
        type: put
      result:
        description: This is a default description.
        type: put
  PeerChannelDiagnostics:
    properties:
      kind:
        description: This is a default description.
        type: put
      numMessagesLost:
        description: This is a default description.
        type: put
      numMessagesReceived:
        description: This is a default description.
        type: put
      numMessagesSent:
        description: This is a default description.
        type: put
      numSendFailures:
        description: This is a default description.
        type: put
  PeerSessionDiagnostics:
    properties:
      connectedTimestampMillis:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      participantId:
        description: This is a default description.
        type: put
  Played:
    properties:
      autoMatched:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      timeMillis:
        description: This is a default description.
        type: put
  Player:
    properties:
      avatarImageUrl:
        description: This is a default description.
        type: put
      bannerUrlLandscape:
        description: This is a default description.
        type: put
      bannerUrlPortrait:
        description: This is a default description.
        type: put
      displayName:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      name:
        description: This is a default description.
        type: put
      originalPlayerId:
        description: This is a default description.
        type: put
      playerId:
        description: This is a default description.
        type: put
      title:
        description: This is a default description.
        type: put
  PlayerAchievement:
    properties:
      achievementState:
        description: This is a default description.
        type: put
      currentSteps:
        description: This is a default description.
        type: put
      experiencePoints:
        description: This is a default description.
        type: put
      formattedCurrentStepsString:
        description: This is a default description.
        type: put
      id:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      lastUpdatedTimestamp:
        description: This is a default description.
        type: put
  PlayerAchievementListResponse:
    properties:
      items:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      nextPageToken:
        description: This is a default description.
        type: put
  PlayerEvent:
    properties:
      definitionId:
        description: This is a default description.
        type: put
      formattedNumEvents:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      numEvents:
        description: This is a default description.
        type: put
      playerId:
        description: This is a default description.
        type: put
  PlayerEventListResponse:
    properties:
      items:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      nextPageToken:
        description: This is a default description.
        type: put
  PlayerExperienceInfo:
    properties:
      currentExperiencePoints:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      lastLevelUpTimestampMillis:
        description: This is a default description.
        type: put
  PlayerLeaderboardScore:
    properties:
      kind:
        description: This is a default description.
        type: put
      leaderboard_id:
        description: This is a default description.
        type: put
      scoreString:
        description: This is a default description.
        type: put
      scoreTag:
        description: This is a default description.
        type: put
      scoreValue:
        description: This is a default description.
        type: put
      timeSpan:
        description: This is a default description.
        type: put
      writeTimestamp:
        description: This is a default description.
        type: put
  PlayerLeaderboardScoreListResponse:
    properties:
      items:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      nextPageToken:
        description: This is a default description.
        type: put
  PlayerLevel:
    properties:
      kind:
        description: This is a default description.
        type: put
      level:
        description: This is a default description.
        type: put
      maxExperiencePoints:
        description: This is a default description.
        type: put
      minExperiencePoints:
        description: This is a default description.
        type: put
  PlayerListResponse:
    properties:
      items:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      nextPageToken:
        description: This is a default description.
        type: put
  PlayerScore:
    properties:
      formattedScore:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      score:
        description: This is a default description.
        type: put
      scoreTag:
        description: This is a default description.
        type: put
      timeSpan:
        description: This is a default description.
        type: put
  PlayerScoreListResponse:
    properties:
      kind:
        description: This is a default description.
        type: put
      submittedScores:
        description: This is a default description.
        type: put
  PlayerScoreResponse:
    properties:
      beatenScoreTimeSpans:
        description: This is a default description.
        type: put
      formattedScore:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      leaderboardId:
        description: This is a default description.
        type: put
      scoreTag:
        description: This is a default description.
        type: put
      unbeatenScores:
        description: This is a default description.
        type: put
  PlayerScoreSubmissionList:
    properties:
      kind:
        description: This is a default description.
        type: put
      scores:
        description: This is a default description.
        type: put
  ProfileSettings:
    properties:
      kind:
        description: This is a default description.
        type: put
      profileVisible:
        description: This is a default description.
        type: put
  PushToken:
    properties:
      clientRevision:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      language:
        description: This is a default description.
        type: put
  PushTokenId:
    properties:
      ios:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
  Quest:
    properties:
      acceptedTimestampMillis:
        description: This is a default description.
        type: put
      applicationId:
        description: This is a default description.
        type: put
      bannerUrl:
        description: This is a default description.
        type: put
      description:
        description: This is a default description.
        type: put
      endTimestampMillis:
        description: This is a default description.
        type: put
      iconUrl:
        description: This is a default description.
        type: put
      id:
        description: This is a default description.
        type: put
      isDefaultBannerUrl:
        description: This is a default description.
        type: put
      isDefaultIconUrl:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
  QuestContribution:
    properties:
      formattedValue:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      value:
        description: This is a default description.
        type: put
  QuestCriterion:
    properties:
      eventId:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
  QuestListResponse:
    properties:
      items:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      nextPageToken:
        description: This is a default description.
        type: put
  QuestMilestone:
    properties:
      completionRewardData:
        description: This is a default description.
        type: put
      criteria:
        description: This is a default description.
        type: put
      id:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      state:
        description: This is a default description.
        type: put
  RevisionCheckResponse:
    properties:
      apiVersion:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      revisionStatus:
        description: This is a default description.
        type: put
  Room:
    properties:
      applicationId:
        description: This is a default description.
        type: put
      description:
        description: This is a default description.
        type: put
      inviterId:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      participants:
        description: This is a default description.
        type: put
      roomId:
        description: This is a default description.
        type: put
      roomStatusVersion:
        description: This is a default description.
        type: put
      status:
        description: This is a default description.
        type: put
      variant:
        description: This is a default description.
        type: put
  RoomAutoMatchStatus:
    properties:
      kind:
        description: This is a default description.
        type: put
      waitEstimateSeconds:
        description: This is a default description.
        type: put
  RoomAutoMatchingCriteria:
    properties:
      exclusiveBitmask:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      maxAutoMatchingPlayers:
        description: This is a default description.
        type: put
      minAutoMatchingPlayers:
        description: This is a default description.
        type: put
  RoomClientAddress:
    properties:
      kind:
        description: This is a default description.
        type: put
      xmppAddress:
        description: This is a default description.
        type: put
  RoomCreateRequest:
    properties:
      capabilities:
        description: This is a default description.
        type: put
      invitedPlayerIds:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      requestId:
        description: This is a default description.
        type: put
      variant:
        description: This is a default description.
        type: put
  RoomJoinRequest:
    properties:
      capabilities:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
  RoomLeaveDiagnostics:
    properties:
      androidNetworkSubtype:
        description: This is a default description.
        type: put
      androidNetworkType:
        description: This is a default description.
        type: put
      iosNetworkType:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      networkOperatorCode:
        description: This is a default description.
        type: put
      networkOperatorName:
        description: This is a default description.
        type: put
      peerSession:
        description: This is a default description.
        type: put
      socketsUsed:
        description: This is a default description.
        type: put
  RoomLeaveRequest:
    properties:
      kind:
        description: This is a default description.
        type: put
      reason:
        description: This is a default description.
        type: put
  RoomList:
    properties:
      items:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      nextPageToken:
        description: This is a default description.
        type: put
  RoomModification:
    properties:
      kind:
        description: This is a default description.
        type: put
      modifiedTimestampMillis:
        description: This is a default description.
        type: put
      participantId:
        description: This is a default description.
        type: put
  RoomP2PStatus:
    properties:
      connectionSetupLatencyMillis:
        description: This is a default description.
        type: put
      error:
        description: This is a default description.
        type: put
      error_reason:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      participantId:
        description: This is a default description.
        type: put
      status:
        description: This is a default description.
        type: put
      unreliableRoundtripLatencyMillis:
        description: This is a default description.
        type: put
  RoomP2PStatuses:
    properties:
      kind:
        description: This is a default description.
        type: put
      updates:
        description: This is a default description.
        type: put
  RoomParticipant:
    properties:
      autoMatched:
        description: This is a default description.
        type: put
      capabilities:
        description: This is a default description.
        type: put
      connected:
        description: This is a default description.
        type: put
      id:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      leaveReason:
        description: This is a default description.
        type: put
      status:
        description: This is a default description.
        type: put
  RoomStatus:
    properties:
      kind:
        description: This is a default description.
        type: put
      participants:
        description: This is a default description.
        type: put
      roomId:
        description: This is a default description.
        type: put
      status:
        description: This is a default description.
        type: put
      statusVersion:
        description: This is a default description.
        type: put
  ScoreSubmission:
    properties:
      kind:
        description: This is a default description.
        type: put
      leaderboardId:
        description: This is a default description.
        type: put
      score:
        description: This is a default description.
        type: put
      scoreTag:
        description: This is a default description.
        type: put
      signature:
        description: This is a default description.
        type: put
  Snapshot:
    properties:
      description:
        description: This is a default description.
        type: put
      driveId:
        description: This is a default description.
        type: put
      durationMillis:
        description: This is a default description.
        type: put
      id:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      lastModifiedMillis:
        description: This is a default description.
        type: put
      progressValue:
        description: This is a default description.
        type: put
      title:
        description: This is a default description.
        type: put
      type:
        description: This is a default description.
        type: put
      uniqueName:
        description: This is a default description.
        type: put
  SnapshotImage:
    properties:
      height:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      mime_type:
        description: This is a default description.
        type: put
      url:
        description: This is a default description.
        type: put
      width:
        description: This is a default description.
        type: put
  SnapshotListResponse:
    properties:
      items:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      nextPageToken:
        description: This is a default description.
        type: put
  TurnBasedAutoMatchingCriteria:
    properties:
      exclusiveBitmask:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      maxAutoMatchingPlayers:
        description: This is a default description.
        type: put
      minAutoMatchingPlayers:
        description: This is a default description.
        type: put
  TurnBasedMatch:
    properties:
      applicationId:
        description: This is a default description.
        type: put
      description:
        description: This is a default description.
        type: put
      inviterId:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      matchId:
        description: This is a default description.
        type: put
      matchNumber:
        description: This is a default description.
        type: put
      matchVersion:
        description: This is a default description.
        type: put
      participants:
        description: This is a default description.
        type: put
      pendingParticipantId:
        description: This is a default description.
        type: put
      rematchId:
        description: This is a default description.
        type: put
  TurnBasedMatchCreateRequest:
    properties:
      invitedPlayerIds:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      requestId:
        description: This is a default description.
        type: put
      variant:
        description: This is a default description.
        type: put
  TurnBasedMatchData:
    properties:
      data:
        description: This is a default description.
        type: put
      dataAvailable:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
  TurnBasedMatchDataRequest:
    properties:
      data:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
  TurnBasedMatchList:
    properties:
      items:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      nextPageToken:
        description: This is a default description.
        type: put
  TurnBasedMatchModification:
    properties:
      kind:
        description: This is a default description.
        type: put
      modifiedTimestampMillis:
        description: This is a default description.
        type: put
      participantId:
        description: This is a default description.
        type: put
  TurnBasedMatchParticipant:
    properties:
      autoMatched:
        description: This is a default description.
        type: put
      id:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      status:
        description: This is a default description.
        type: put
  TurnBasedMatchRematch:
    properties:
      kind:
        description: This is a default description.
        type: put
  TurnBasedMatchResults:
    properties:
      kind:
        description: This is a default description.
        type: put
      matchVersion:
        description: This is a default description.
        type: put
      results:
        description: This is a default description.
        type: put
  TurnBasedMatchSync:
    properties:
      items:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      moreAvailable:
        description: This is a default description.
        type: put
      nextPageToken:
        description: This is a default description.
        type: put
  TurnBasedMatchTurn:
    properties:
      kind:
        description: This is a default description.
        type: put
      matchVersion:
        description: This is a default description.
        type: put
      pendingParticipantId:
        description: This is a default description.
        type: put
      results:
        description: This is a default description.
        type: put
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---