---
trigger: always_on
---

# Mintlify technical writing assistant

## Mintlify component reference

### API documentation components

#### Parameter fields

<ParamField path="user_id" type="string" required>
Unique identifier for the user. Must be a valid UUID v4 format.
</ParamField>

<ParamField body="email" type="string" required>
User's email address. Must be valid and unique within the system.
</ParamField>

<ParamField query="limit" type="integer" default="10">
Maximum number of results to return. Range: 1-100.
</ParamField>

<ParamField header="Authorization" type="string" required>
Bearer token for API authentication. Format: `Bearer YOUR_API_KEY`
</ParamField>

#### Response fields

<ResponseField name="user_id" type="string" required>
Unique identifier assigned to the newly created user.
</ResponseField>

<ResponseField name="created_at" type="timestamp">
ISO 8601 formatted timestamp of when the user was created.
</ResponseField>

<ResponseField name="permissions" type="array">
List of permission strings assigned to this user.
</ResponseField>

#### Expandable nested fields

<ResponseField name="user" type="object">
Complete user object with all associated data.

<Expandable title="User properties">
    <ResponseField name="profile" type="object">
    User profile information including personal details.
    
    <Expandable title="Profile details">
        <ResponseField name="first_name" type="string">
        User's first name as entered during registration.
        </ResponseField>
        
        <ResponseField name="avatar_url" type="string | null">
        URL to user's profile picture. Returns null if no avatar is set.
        </ResponseField>
    </Expandable>
    </ResponseField>
</Expandable>
</ResponseField>