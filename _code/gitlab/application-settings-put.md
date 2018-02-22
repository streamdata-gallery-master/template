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
  /application/settings:
    put:
      summary: Put Application Settings
      description: Modify application settings
      operationId: putV3ApplicationSettings
      parameters:
      - in: formData
        name: admin_notification_email
        description: Abuse reports will be sent to this address if it is set
      - in: formData
        name: after_sign_out_path
        description: We will redirect users to this page after they sign out
      - in: formData
        name: after_sign_up_text
        description: Text shown after sign up
      - in: formData
        name: akismet_api_key
        description: Generate API key at http://www
      - in: formData
        name: akismet_enabled
        description: Helps prevent bots from creating issues
      - in: formData
        name: container_registry_token_expire_delay
        description: Authorization token duration (minutes)
      - in: formData
        name: default_branch_protection
        description: Determine if developers can push to master
      - in: formData
        name: default_group_visibility
        description: The default group visibility
      - in: formData
        name: default_projects_limit
        description: The maximum number of personal projects
      - in: formData
        name: default_project_visibility
        description: The default project visibility
      - in: formData
        name: default_snippet_visibility
        description: The default snippet visibility
      - in: formData
        name: disabled_oauth_sign_in_sources
        description: Disable certain OAuth sign-in sources
      - in: formData
        name: domain_blacklist
        description: Users with e-mail addresses that match these domain(s) will NOT
          be able to sign-up
      - in: formData
        name: domain_blacklist_enabled
        description: Enable domain blacklist for sign ups
      - in: formData
        name: domain_whitelist
        description: ONLY users with e-mail addresses that match these domain(s) will
          be able to sign-up
      - in: formData
        name: email_author_in_body
        description: Some email servers do not support overriding the email sender
          name
      - in: formData
        name: enabled_git_access_protocol
        description: Allow only the selected protocols to be used for Git access
      - in: formData
        name: gravatar_enabled
        description: Flag indicating if the Gravatar service is enabled
      - in: formData
        name: help_page_text
        description: Custom text displayed on the help page
      - in: formData
        name: home_page_url
        description: We will redirect non-logged in users to this page
      - in: formData
        name: housekeeping_bitmaps_enabled
        description: Creating pack file bitmaps makes housekeeping take a little longer
          but bitmaps should accelerate 'git clone' performance
      - in: formData
        name: housekeeping_enabled
        description: Enable automatic repository housekeeping (git repack, git gc)
      - in: formData
        name: housekeeping_full_repack_period
        description: Number of Git pushes after which a full 'git repack' is run
      - in: formData
        name: housekeeping_gc_period
        description: Number of Git pushes after which 'git gc' is run
      - in: formData
        name: housekeeping_incremental_repack_period
        description: Number of Git pushes after which an incremental 'git repack'
          is run
      - in: formData
        name: html_emails_enabled
        description: By default GitLab sends emails in HTML and plain text formats
          so mail clients can choose what format to use
      - in: formData
        name: import_sources
        description: Enabled sources for code import during project creation
      - in: formData
        name: koding_enabled
        description: Enable Koding
      - in: formData
        name: koding_url
        description: The Koding team URL
      - in: formData
        name: max_artifacts_size
        description: Set the maximum file size each build's artifacts can have
      - in: formData
        name: max_attachment_size
        description: Maximum attachment size in MB
      - in: formData
        name: metrics_enabled
        description: Enable the InfluxDB metrics
      - in: formData
        name: metrics_host
        description: The InfluxDB host
      - in: formData
        name: metrics_method_call_threshold
        description: A method call is only tracked when it takes longer to complete
          than the given amount of milliseconds
      - in: formData
        name: metrics_packet_size
        description: The amount of points to store in a single UDP packet
      - in: formData
        name: metrics_pool_size
        description: The amount of InfluxDB connections to open
      - in: formData
        name: metrics_port
        description: The UDP port to use for connecting to InfluxDB
      - in: formData
        name: metrics_sample_interval
        description: The sampling interval in seconds
      - in: formData
        name: metrics_timeout
        description: The amount of seconds after which an InfluxDB connection will
          time out
      - in: formData
        name: plantuml_enabled
        description: Enable PlantUML
      - in: formData
        name: plantuml_url
        description: The PlantUML server URL
      - in: formData
        name: recaptcha_enabled
        description: Helps prevent bots from creating accounts
      - in: formData
        name: recaptcha_private_key
        description: Generate private key at http://www
      - in: formData
        name: recaptcha_site_key
        description: Generate site key at http://www
      - in: formData
        name: repository_checks_enabled
        description: GitLab will periodically run 'git fsck' in all project and wiki
          repositories to look for silent disk corruption issues
      - in: formData
        name: repository_storage
        description: Storage paths for new projects
      - in: formData
        name: require_two_factor_authentication
        description: Require all users to setup Two-factor authentication
      - in: formData
        name: restricted_visibility_levels
        description: Selected levels cannot be used by non-admin users for projects
          or snippets
      - in: formData
        name: send_user_confirmation_email
        description: Send confirmation email on sign-up
      - in: formData
        name: sentry_dsn
        description: Sentry Data Source Name
      - in: formData
        name: sentry_enabled
        description: 'Sentry is an error reporting and logging tool which is currently
          not shipped with GitLab, get it here: https://getsentry'
      - in: formData
        name: session_expire_delay
        description: Session duration in minutes
      - in: formData
        name: shared_runners_enabled
        description: Enable shared runners for new projects
      - in: formData
        name: shared_runners_text
        description: 'Shared runners text '
      - in: formData
        name: sidekiq_throttling_enabled
        description: Enable Sidekiq Job Throttling
      - in: formData
        name: sidekiq_throttling_factor
        description: The factor by which the queues should be throttled
      - in: formData
        name: sidekiq_throttling_queus
        description: Choose which queues you wish to throttle
      - in: formData
        name: signin_enabled
        description: Flag indicating if sign in is enabled
      - in: formData
        name: signup_enabled
        description: Flag indicating if sign up is enabled
      - in: formData
        name: sign_in_text
        description: The sign in text of the GitLab application
      - in: formData
        name: two_factor_grace_period
        description: Amount of time (in hours) that users are allowed to skip forced
          configuration of two-factor authentication
      - in: formData
        name: user_default_external
        description: Newly registered users will by default be external
      - in: formData
        name: user_oauth_applications
        description: Allow users to register any application to use GitLab as an OAuth
          provider
      - in: formData
        name: version_check_enabled
        description: Let GitLab inform you when an update is available
      responses:
        200:
          description: OK
      tags:
      - application
      - settings
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