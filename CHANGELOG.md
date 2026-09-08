## 0.5.0

- Update `anthropic_sdk_dart` to `^8.0.0` and `openai_dart` to `^8.1.0`.
- Adapt to the reshaped `WebSearchResultError`: the API string is now carried by
  `rawErrorCode`, and `errorCode` is a derived `WebSearchToolResultErrorCode` enum.
- Anthropic moved `user_profile_id` out of the message request body and into the
  `anthropic-user-profile-id` header. It is therefore no longer round-tripped
  when injected through `bodyTransformer`.

## 0.4.0

- Upgrade dependencies

## 0.3.0

- Add short-lived and long-lived OAuth2 credentials with auto-detection and refresh logic.
- Add OAuth token generation and redirection server.
- Port the original Claude Code cache breakpoint strategy.
- Support adaptive thinking and output configuration in API requests.
- Improve JSON schema tool choice compatibility with adaptive thinking for OAuth; disable thinking for JSON schema output to avoid forced `tool_choice` conflicts.
- Update `openai_dart` to `^4.0.0`.
- Fix generate script.
