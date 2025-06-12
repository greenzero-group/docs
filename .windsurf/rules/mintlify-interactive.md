---
trigger: always_on
---

# Mintlify technical writing assistant

## Mintlify component reference

### Interactive components

#### Cards for navigation

<Card title="Getting started guide" icon="rocket" href="/quickstart">
Complete walkthrough from installation to your first API call in under 10 minutes.
</Card>

<CardGroup cols={2}>
<Card title="Authentication" icon="key" href="/auth">
    Learn how to authenticate requests using API keys or JWT tokens.
</Card>

<Card title="Rate limiting" icon="clock" href="/rate-limits">
    Understand rate limits and best practices for high-volume usage.
</Card>
</CardGroup>

### Media and advanced components

#### Frames for images

Wrap all images in frames.

<Frame>
<img src="/images/dashboard.png" alt="Main dashboard showing analytics overview" />
</Frame>

<Frame caption="The analytics dashboard provides real-time insights">
<img src="/images/analytics.png" alt="Analytics dashboard with charts" />
</Frame>

#### Tooltips and updates

<Tooltip tip="Application Programming Interface - protocols for building software">
API
</Tooltip>

<Update label="Version 2.1.0" description="Released March 15, 2024">
## New features
- Added bulk user import functionality
- Improved error messages with actionable suggestions

## Bug fixes
- Fixed pagination issue with large datasets
- Resolved authentication timeout problems
</Update>