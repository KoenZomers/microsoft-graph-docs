```typescript
const options = {
	authProvider,
};

const client = Client.init(options);

let events = await client.api('/me/events')
	.header('Prefer','outlook.timezone="Pacific Standard Time"')
	.select('subject,body,bodyPreview,organizer,attendees,start,end,location')
	.get();
```