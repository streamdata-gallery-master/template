---
swagger: "2.0"
info:
  title: GitLab
  description: 'GitLab Inc. is a company based on the GitLab open-source project,
    helping developers collaborate on code to build great things and ship on time.
    We are an active participant in our global community of customers and contributors,
    trying to serve their needs and lead by example. We have one vision: everyone
    can contribute to all digital content, and our mission is to change all creative
    work from read-only to read-write.'
  version: 1.0.0
host: gitlab.com
basePath: v3/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/{id}/block:
    put:
      summary: Put Users  Block
      description: Block a user
      operationId: putV3UsersIdBlock
      parameters:
      - in: path
        name: id
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - users
      - ""
      - block
definitions:
  AccessRequester:
    properties:
      avatar_url:
        description: This is a default description.
        type: get
      id:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      requested_at:
        description: This is a default description.
        type: get
      state:
        description: This is a default description.
        type: get
      username:
        description: This is a default description.
        type: get
      web_url:
        description: This is a default description.
        type: get
  ApplicationSetting:
    properties:
      after_sign_out_path:
        description: This is a default description.
        type: get
      after_sign_up_text:
        description: This is a default description.
        type: get
      container_registry_token_expire_delay:
        description: This is a default description.
        type: get
      created_at:
        description: This is a default description.
        type: get
      default_branch_protection:
        description: This is a default description.
        type: get
      default_group_visibility:
        description: This is a default description.
        type: get
      default_project_visibility:
        description: This is a default description.
        type: get
      default_projects_limit:
        description: This is a default description.
        type: get
      default_snippet_visibility:
        description: This is a default description.
        type: get
      domain_blacklist:
        description: This is a default description.
        type: get
  AwardEmoji:
    properties:
      awardable_id:
        description: This is a default description.
        type: get
      awardable_type:
        description: This is a default description.
        type: get
      created_at:
        description: This is a default description.
        type: get
      id:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      updated_at:
        description: This is a default description.
        type: get
  BasicProjectDetails:
    properties:
      http_url_to_repo:
        description: This is a default description.
        type: get
      id:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      name_with_namespace:
        description: This is a default description.
        type: get
      path:
        description: This is a default description.
        type: get
      path_with_namespace:
        description: This is a default description.
        type: get
      web_url:
        description: This is a default description.
        type: get
  Board:
    properties:
      id:
        description: This is a default description.
        type: get
  Build:
    properties:
      coverage:
        description: This is a default description.
        type: get
      created_at:
        description: This is a default description.
        type: get
      finished_at:
        description: This is a default description.
        type: get
      id:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      ref:
        description: This is a default description.
        type: get
      stage:
        description: This is a default description.
        type: get
      started_at:
        description: This is a default description.
        type: get
      status:
        description: This is a default description.
        type: get
      tag:
        description: This is a default description.
        type: get
  BuildArtifactFile:
    properties:
      filename:
        description: This is a default description.
        type: get
      size:
        description: This is a default description.
        type: get
  CommitNote:
    properties:
      created_at:
        description: This is a default description.
        type: get
      line:
        description: This is a default description.
        type: get
      line_type:
        description: This is a default description.
        type: get
      note:
        description: This is a default description.
        type: get
      path:
        description: This is a default description.
        type: get
  CommitStatus:
    properties:
      allow_failure:
        description: This is a default description.
        type: get
      created_at:
        description: This is a default description.
        type: get
      description:
        description: This is a default description.
        type: get
      finished_at:
        description: This is a default description.
        type: get
      id:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      ref:
        description: This is a default description.
        type: get
      sha:
        description: This is a default description.
        type: get
      started_at:
        description: This is a default description.
        type: get
      status:
        description: This is a default description.
        type: get
  Compare:
    properties:
      compare_same_ref:
        description: This is a default description.
        type: get
      compare_timeout:
        description: This is a default description.
        type: get
  Contributor:
    properties:
      additions:
        description: This is a default description.
        type: get
      commits:
        description: This is a default description.
        type: get
      deletions:
        description: This is a default description.
        type: get
      email:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
  Deployment:
    properties:
      created_at:
        description: This is a default description.
        type: get
      id:
        description: This is a default description.
        type: get
      iid:
        description: This is a default description.
        type: get
      ref:
        description: This is a default description.
        type: get
      sha:
        description: This is a default description.
        type: get
  Email:
    properties:
      email:
        description: This is a default description.
        type: get
      id:
        description: This is a default description.
        type: get
  Environment:
    properties:
      external_url:
        description: This is a default description.
        type: get
      id:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      slug:
        description: This is a default description.
        type: get
  EnvironmentBasic:
    properties:
      external_url:
        description: This is a default description.
        type: get
      id:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      slug:
        description: This is a default description.
        type: get
  Event:
    properties:
      action_name:
        description: This is a default description.
        type: get
      author_id:
        description: This is a default description.
        type: get
      author_username:
        description: This is a default description.
        type: get
      created_at:
        description: This is a default description.
        type: get
      data:
        description: This is a default description.
        type: get
      project_id:
        description: This is a default description.
        type: get
      target_id:
        description: This is a default description.
        type: get
      target_title:
        description: This is a default description.
        type: get
      target_type:
        description: This is a default description.
        type: get
      title:
        description: This is a default description.
        type: get
  GlobalNotificationSetting:
    properties:
      events:
        description: This is a default description.
        type: get
      level:
        description: This is a default description.
        type: get
      notification_email:
        description: This is a default description.
        type: get
  Group:
    properties:
      avatar_url:
        description: This is a default description.
        type: get
      description:
        description: This is a default description.
        type: get
      id:
        description: This is a default description.
        type: get
      lfs_enabled:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      path:
        description: This is a default description.
        type: get
      request_access_enabled:
        description: This is a default description.
        type: get
      statistics:
        description: This is a default description.
        type: get
      visibility_level:
        description: This is a default description.
        type: get
      web_url:
        description: This is a default description.
        type: get
  GroupDetail:
    properties:
      avatar_url:
        description: This is a default description.
        type: get
      description:
        description: This is a default description.
        type: get
      id:
        description: This is a default description.
        type: get
      lfs_enabled:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      path:
        description: This is a default description.
        type: get
      request_access_enabled:
        description: This is a default description.
        type: get
      statistics:
        description: This is a default description.
        type: get
      visibility_level:
        description: This is a default description.
        type: get
      web_url:
        description: This is a default description.
        type: get
  Hook:
    properties:
      created_at:
        description: This is a default description.
        type: get
      enable_ssl_verification:
        description: This is a default description.
        type: get
      id:
        description: This is a default description.
        type: get
      push_events:
        description: This is a default description.
        type: get
      tag_push_events:
        description: This is a default description.
        type: get
      url:
        description: This is a default description.
        type: get
  Identity:
    properties:
      extern_uid:
        description: This is a default description.
        type: get
      provider:
        description: This is a default description.
        type: get
  Issue:
    properties:
      confidential:
        description: This is a default description.
        type: get
      created_at:
        description: This is a default description.
        type: get
      description:
        description: This is a default description.
        type: get
      downvotes:
        description: This is a default description.
        type: get
      due_date:
        description: This is a default description.
        type: get
      id:
        description: This is a default description.
        type: get
      iid:
        description: This is a default description.
        type: get
      labels:
        description: This is a default description.
        type: get
      project_id:
        description: This is a default description.
        type: get
      state:
        description: This is a default description.
        type: get
  Label:
    properties:
      closed_issues_count:
        description: This is a default description.
        type: get
      color:
        description: This is a default description.
        type: get
      description:
        description: This is a default description.
        type: get
      id:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      open_issues_count:
        description: This is a default description.
        type: get
      open_merge_requests_count:
        description: This is a default description.
        type: get
      priority:
        description: This is a default description.
        type: get
      subscribed:
        description: This is a default description.
        type: get
  LabelBasic:
    properties:
      color:
        description: This is a default description.
        type: get
      description:
        description: This is a default description.
        type: get
      id:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
  List:
    properties:
      id:
        description: This is a default description.
        type: get
      position:
        description: This is a default description.
        type: get
  MRNote:
    properties:
      note:
        description: This is a default description.
        type: get
  Member:
    properties:
      access_level:
        description: This is a default description.
        type: get
      avatar_url:
        description: This is a default description.
        type: get
      expires_at:
        description: This is a default description.
        type: get
      id:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      state:
        description: This is a default description.
        type: get
      username:
        description: This is a default description.
        type: get
      web_url:
        description: This is a default description.
        type: get
  MergeRequest:
    properties:
      created_at:
        description: This is a default description.
        type: get
      description:
        description: This is a default description.
        type: get
      downvotes:
        description: This is a default description.
        type: get
      force_remove_source_branch:
        description: This is a default description.
        type: get
      id:
        description: This is a default description.
        type: get
      iid:
        description: This is a default description.
        type: get
      labels:
        description: This is a default description.
        type: get
      merge_commit_sha:
        description: This is a default description.
        type: get
      merge_status:
        description: This is a default description.
        type: get
      merge_when_build_succeeds:
        description: This is a default description.
        type: get
  MergeRequestChanges:
    properties:
      created_at:
        description: This is a default description.
        type: get
      description:
        description: This is a default description.
        type: get
      downvotes:
        description: This is a default description.
        type: get
      force_remove_source_branch:
        description: This is a default description.
        type: get
      id:
        description: This is a default description.
        type: get
      iid:
        description: This is a default description.
        type: get
      labels:
        description: This is a default description.
        type: get
      merge_commit_sha:
        description: This is a default description.
        type: get
      merge_status:
        description: This is a default description.
        type: get
      merge_when_build_succeeds:
        description: This is a default description.
        type: get
  MergeRequestDiff:
    properties:
      base_commit_sha:
        description: This is a default description.
        type: get
      created_at:
        description: This is a default description.
        type: get
      head_commit_sha:
        description: This is a default description.
        type: get
      id:
        description: This is a default description.
        type: get
      merge_request_id:
        description: This is a default description.
        type: get
      real_size:
        description: This is a default description.
        type: get
      start_commit_sha:
        description: This is a default description.
        type: get
      state:
        description: This is a default description.
        type: get
  MergeRequestDiffFull:
    properties:
      base_commit_sha:
        description: This is a default description.
        type: get
      created_at:
        description: This is a default description.
        type: get
      head_commit_sha:
        description: This is a default description.
        type: get
      id:
        description: This is a default description.
        type: get
      merge_request_id:
        description: This is a default description.
        type: get
      real_size:
        description: This is a default description.
        type: get
      start_commit_sha:
        description: This is a default description.
        type: get
      state:
        description: This is a default description.
        type: get
  Milestone:
    properties:
      created_at:
        description: This is a default description.
        type: get
      description:
        description: This is a default description.
        type: get
      due_date:
        description: This is a default description.
        type: get
      id:
        description: This is a default description.
        type: get
      iid:
        description: This is a default description.
        type: get
      project_id:
        description: This is a default description.
        type: get
      start_date:
        description: This is a default description.
        type: get
      state:
        description: This is a default description.
        type: get
      title:
        description: This is a default description.
        type: get
      updated_at:
        description: This is a default description.
        type: get
  Namespace:
    properties:
      id:
        description: This is a default description.
        type: get
      kind:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      path:
        description: This is a default description.
        type: get
  Note:
    properties:
      attachment:
        description: This is a default description.
        type: get
      body:
        description: This is a default description.
        type: get
      created_at:
        description: This is a default description.
        type: get
      downvote?:
        description: This is a default description.
        type: get
      id:
        description: This is a default description.
        type: get
      noteable_id:
        description: This is a default description.
        type: get
      noteable_type:
        description: This is a default description.
        type: get
      system:
        description: This is a default description.
        type: get
      updated_at:
        description: This is a default description.
        type: get
      upvote?:
        description: This is a default description.
        type: get
  NotificationSetting:
    properties:
      events:
        description: This is a default description.
        type: get
      level:
        description: This is a default description.
        type: get
  PersonalSnippet:
    properties:
      created_at:
        description: This is a default description.
        type: get
      file_name:
        description: This is a default description.
        type: get
      id:
        description: This is a default description.
        type: get
      raw_url:
        description: This is a default description.
        type: get
      title:
        description: This is a default description.
        type: get
      updated_at:
        description: This is a default description.
        type: get
      web_url:
        description: This is a default description.
        type: get
  Pipeline:
    properties:
      before_sha:
        description: This is a default description.
        type: get
      committed_at:
        description: This is a default description.
        type: get
      coverage:
        description: This is a default description.
        type: get
      created_at:
        description: This is a default description.
        type: get
      duration:
        description: This is a default description.
        type: get
      finished_at:
        description: This is a default description.
        type: get
      id:
        description: This is a default description.
        type: get
      ref:
        description: This is a default description.
        type: get
      sha:
        description: This is a default description.
        type: get
      started_at:
        description: This is a default description.
        type: get
  PipelineBasic:
    properties:
      id:
        description: This is a default description.
        type: get
      ref:
        description: This is a default description.
        type: get
      sha:
        description: This is a default description.
        type: get
      status:
        description: This is a default description.
        type: get
  Project:
    properties:
      archived:
        description: This is a default description.
        type: get
      avatar_url:
        description: This is a default description.
        type: get
      builds_enabled:
        description: This is a default description.
        type: get
      container_registry_enabled:
        description: This is a default description.
        type: get
      created_at:
        description: This is a default description.
        type: get
      creator_id:
        description: This is a default description.
        type: get
      default_branch:
        description: This is a default description.
        type: get
      description:
        description: This is a default description.
        type: get
      forks_count:
        description: This is a default description.
        type: get
      http_url_to_repo:
        description: This is a default description.
        type: get
  ProjectGroupLink:
    properties:
      expires_at:
        description: This is a default description.
        type: get
      group_access:
        description: This is a default description.
        type: get
      group_id:
        description: This is a default description.
        type: get
      id:
        description: This is a default description.
        type: get
      project_id:
        description: This is a default description.
        type: get
  ProjectHook:
    properties:
      build_events:
        description: This is a default description.
        type: get
      created_at:
        description: This is a default description.
        type: get
      enable_ssl_verification:
        description: This is a default description.
        type: get
      id:
        description: This is a default description.
        type: get
      issues_events:
        description: This is a default description.
        type: get
      merge_requests_events:
        description: This is a default description.
        type: get
      note_events:
        description: This is a default description.
        type: get
      pipeline_events:
        description: This is a default description.
        type: get
      project_id:
        description: This is a default description.
        type: get
      push_events:
        description: This is a default description.
        type: get
  ProjectService:
    properties:
      active:
        description: This is a default description.
        type: get
      build_events:
        description: This is a default description.
        type: get
      created_at:
        description: This is a default description.
        type: get
      id:
        description: This is a default description.
        type: get
      issues_events:
        description: This is a default description.
        type: get
      merge_requests_events:
        description: This is a default description.
        type: get
      note_events:
        description: This is a default description.
        type: get
      pipeline_events:
        description: This is a default description.
        type: get
      properties:
        description: This is a default description.
        type: get
      push_events:
        description: This is a default description.
        type: get
  ProjectSnippet:
    properties:
      created_at:
        description: This is a default description.
        type: get
      expires_at:
        description: This is a default description.
        type: get
      file_name:
        description: This is a default description.
        type: get
      id:
        description: This is a default description.
        type: get
      title:
        description: This is a default description.
        type: get
      updated_at:
        description: This is a default description.
        type: get
      web_url:
        description: This is a default description.
        type: get
  ProjectStatistics:
    properties:
      build_artifacts_size:
        description: This is a default description.
        type: get
      commit_count:
        description: This is a default description.
        type: get
      lfs_objects_size:
        description: This is a default description.
        type: get
      repository_size:
        description: This is a default description.
        type: get
      storage_size:
        description: This is a default description.
        type: get
  ProjectWithAccess:
    properties:
      archived:
        description: This is a default description.
        type: get
      avatar_url:
        description: This is a default description.
        type: get
      builds_enabled:
        description: This is a default description.
        type: get
      container_registry_enabled:
        description: This is a default description.
        type: get
      created_at:
        description: This is a default description.
        type: get
      creator_id:
        description: This is a default description.
        type: get
      default_branch:
        description: This is a default description.
        type: get
      description:
        description: This is a default description.
        type: get
      forks_count:
        description: This is a default description.
        type: get
      http_url_to_repo:
        description: This is a default description.
        type: get
  Release:
    properties:
      description:
        description: This is a default description.
        type: get
      tag_name:
        description: This is a default description.
        type: get
  RepoBranch:
    properties:
      commit:
        description: This is a default description.
        type: get
      developers_can_merge:
        description: This is a default description.
        type: get
      developers_can_push:
        description: This is a default description.
        type: get
      merged:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      protected:
        description: This is a default description.
        type: get
  RepoCommit:
    properties:
      author_email:
        description: This is a default description.
        type: get
      author_name:
        description: This is a default description.
        type: get
      committer_email:
        description: This is a default description.
        type: get
      committer_name:
        description: This is a default description.
        type: get
      created_at:
        description: This is a default description.
        type: get
      id:
        description: This is a default description.
        type: get
      message:
        description: This is a default description.
        type: get
      short_id:
        description: This is a default description.
        type: get
      title:
        description: This is a default description.
        type: get
  RepoCommitDetail:
    properties:
      author_email:
        description: This is a default description.
        type: get
      author_name:
        description: This is a default description.
        type: get
      authored_date:
        description: This is a default description.
        type: get
      committed_date:
        description: This is a default description.
        type: get
      committer_email:
        description: This is a default description.
        type: get
      committer_name:
        description: This is a default description.
        type: get
      created_at:
        description: This is a default description.
        type: get
      id:
        description: This is a default description.
        type: get
      message:
        description: This is a default description.
        type: get
      parent_ids:
        description: This is a default description.
        type: get
  RepoCommitStats:
    properties:
      additions:
        description: This is a default description.
        type: get
      deletions:
        description: This is a default description.
        type: get
      total:
        description: This is a default description.
        type: get
  RepoDiff:
    properties:
      a_mode:
        description: This is a default description.
        type: get
      b_mode:
        description: This is a default description.
        type: get
      deleted_file:
        description: This is a default description.
        type: get
      diff:
        description: This is a default description.
        type: get
      new_file:
        description: This is a default description.
        type: get
      new_path:
        description: This is a default description.
        type: get
      old_path:
        description: This is a default description.
        type: get
      renamed_file:
        description: This is a default description.
        type: get
  RepoLicense:
    properties:
      conditions:
        description: This is a default description.
        type: get
      content:
        description: This is a default description.
        type: get
      description:
        description: This is a default description.
        type: get
      html_url:
        description: This is a default description.
        type: get
      key:
        description: This is a default description.
        type: get
      limitations:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      nickname:
        description: This is a default description.
        type: get
      permissions:
        description: This is a default description.
        type: get
      popular:
        description: This is a default description.
        type: get
  RepoTag:
    properties:
      commit:
        description: This is a default description.
        type: get
      message:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
  RepoTreeObject:
    properties:
      id:
        description: This is a default description.
        type: get
      mode:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      path:
        description: This is a default description.
        type: get
      type:
        description: This is a default description.
        type: get
  Runner:
    properties:
      active:
        description: This is a default description.
        type: get
      description:
        description: This is a default description.
        type: get
      id:
        description: This is a default description.
        type: get
      is_shared:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
  RunnerDetails:
    properties:
      active:
        description: This is a default description.
        type: get
      architecture:
        description: This is a default description.
        type: get
      contacted_at:
        description: This is a default description.
        type: get
      description:
        description: This is a default description.
        type: get
      id:
        description: This is a default description.
        type: get
      is_shared:
        description: This is a default description.
        type: get
      locked:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      platform:
        description: This is a default description.
        type: get
      revision:
        description: This is a default description.
        type: get
  SSHKey:
    properties:
      can_push:
        description: This is a default description.
        type: get
      created_at:
        description: This is a default description.
        type: get
      id:
        description: This is a default description.
        type: get
      key:
        description: This is a default description.
        type: get
      title:
        description: This is a default description.
        type: get
  SSHKeyWithUser:
    properties:
      can_push:
        description: This is a default description.
        type: get
      created_at:
        description: This is a default description.
        type: get
      id:
        description: This is a default description.
        type: get
      key:
        description: This is a default description.
        type: get
      title:
        description: This is a default description.
        type: get
  Template:
    properties:
      content:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
  TemplatesList:
    properties:
      name:
        description: This is a default description.
        type: get
  Todo:
    properties:
      action_name:
        description: This is a default description.
        type: get
      body:
        description: This is a default description.
        type: get
      created_at:
        description: This is a default description.
        type: get
      id:
        description: This is a default description.
        type: get
      state:
        description: This is a default description.
        type: get
      target:
        description: This is a default description.
        type: get
      target_type:
        description: This is a default description.
        type: get
      target_url:
        description: This is a default description.
        type: get
  Trigger:
    properties:
      created_at:
        description: This is a default description.
        type: get
      deleted_at:
        description: This is a default description.
        type: get
      last_used:
        description: This is a default description.
        type: get
      token:
        description: This is a default description.
        type: get
      updated_at:
        description: This is a default description.
        type: get
  TriggerRequest:
    properties:
      id:
        description: This is a default description.
        type: get
      variables:
        description: This is a default description.
        type: get
  User:
    properties:
      avatar_url:
        description: This is a default description.
        type: get
      bio:
        description: This is a default description.
        type: get
      created_at:
        description: This is a default description.
        type: get
      id:
        description: This is a default description.
        type: get
      is_admin:
        description: This is a default description.
        type: get
      linkedin:
        description: This is a default description.
        type: get
      location:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      organization:
        description: This is a default description.
        type: get
      skype:
        description: This is a default description.
        type: get
  UserBasic:
    properties:
      avatar_url:
        description: This is a default description.
        type: get
      id:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      state:
        description: This is a default description.
        type: get
      username:
        description: This is a default description.
        type: get
      web_url:
        description: This is a default description.
        type: get
  UserPublic:
    properties:
      avatar_url:
        description: This is a default description.
        type: get
      bio:
        description: This is a default description.
        type: get
      can_create_group:
        description: This is a default description.
        type: get
      can_create_project:
        description: This is a default description.
        type: get
      color_scheme_id:
        description: This is a default description.
        type: get
      confirmed_at:
        description: This is a default description.
        type: get
      created_at:
        description: This is a default description.
        type: get
      current_sign_in_at:
        description: This is a default description.
        type: get
      email:
        description: This is a default description.
        type: get
      external:
        description: This is a default description.
        type: get
  UserWithPrivateToken:
    properties:
      avatar_url:
        description: This is a default description.
        type: get
      bio:
        description: This is a default description.
        type: get
      can_create_group:
        description: This is a default description.
        type: get
      can_create_project:
        description: This is a default description.
        type: get
      color_scheme_id:
        description: This is a default description.
        type: get
      confirmed_at:
        description: This is a default description.
        type: get
      created_at:
        description: This is a default description.
        type: get
      current_sign_in_at:
        description: This is a default description.
        type: get
      email:
        description: This is a default description.
        type: get
      external:
        description: This is a default description.
        type: get
  Variable:
    properties:
      key:
        description: This is a default description.
        type: get
      value:
        description: This is a default description.
        type: get
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