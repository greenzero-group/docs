---
trigger: always_on
---

# Mintlify technical writing assistant

## Mintlify component reference

### Callout components

#### Note - Additional helpful information

<Note>
Supplementary information that supports the main content without interrupting flow
</Note>

#### Tip - Best practices and pro tips

<Tip>
Expert advice, shortcuts, or best practices that enhance user success
</Tip>

#### Warning - Important cautions

<Warning>
Critical information about potential issues, breaking changes, or destructive actions
</Warning>

#### Info - Neutral contextual information

<Info>
Background information, context, or neutral announcements
</Info>

#### Check - Success confirmations

<Check>
Positive confirmations, successful completions, or achievement indicators
</Check>

### Code components

#### Single code block

```javascript config.js
const apiConfig = {
baseURL: 'https://api.example.com',
timeout: 5000,
headers: {
    'Authorization': `Bearer ${process.env.API_TOKEN}`
}
};
```

#### Code group with multiple languages

<CodeGroup>
```javascript Node.js
const response = await fetch('/api/endpoint', {
    headers: { Authorization: `Bearer ${apiKey}` }
});
```

```python Python
import requests
response = requests.get('/api/endpoint', 
    headers={'Authorization': f'Bearer {api_key}'})
```

```curl cURL
curl -X GET '/api/endpoint' \
    -H 'Authorization: Bearer YOUR_API_KEY'
```
</CodeGroup>

#### Request/Response examples

<RequestExample>
```bash cURL
curl -X POST 'https://api.example.com/users' \
    -H 'Content-Type: application/json' \
    -d '{"name": "John Doe", "email": "john@example.com"}'
```
</RequestExample>

<ResponseExample>
```json Success
{
    "id": "user_123",
    "name": "John Doe", 
    "email": "john@example.com",
    "created_at": "2024-01-15T10:30:00Z"
}
```
</ResponseExample>

### Structural components

#### Steps for procedures

<Steps>
<Step title="Install dependencies">
    Run `npm install` to install required packages.
    
    <Check>
    Verify installation by running `npm list`.
    </Check>
</Step>

<Step title="Configure environment">
    Create a `.env` file with your API credentials.
    
    ```bash
    API_KEY=your_api_key_here
    ```
    
    <Warning>
    Never commit API keys to version control.
    </Warning>
</Step>
</Steps>

#### Tabs for alternative content

<Tabs>
<Tab title="macOS">
    ```bash
    brew install node
    npm install -g package-name
    ```
</Tab>

<Tab title="Windows">
    ```powershell
    choco install nodejs
    npm install -g package-name
    ```
</Tab>

<Tab title="Linux">
    ```bash
    sudo apt install nodejs npm
    npm install -g package-name
    ```
</Tab>
</Tabs>

#### Accordions for collapsible content

<AccordionGroup>
<Accordion title="Troubleshooting connection issues">
    - **Firewall blocking**: Ensure ports 80 and 443 are open
    - **Proxy configuration**: Set HTTP_PROXY environment variable
    - **DNS resolution**: Try using 8.8.8.8 as DNS server
</Accordion>

<Accordion title="Advanced configuration">
    ```javascript
    const config = {
    performance: { cache: true, timeout: 30000 },
    security: { encryption: 'AES-256' }
    };
    ```
</Accordion>
</AccordionGroup>