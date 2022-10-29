WEB API Design:


1) REST: Best for APIs that expose CRUD operations (Its all about Resources )
	- CRUD Operations
	- Non-CRUD Operations:
		- Archive
		- Deactivate
		- Search -> Query Params
	- Pros:
		- Standard Methods
		- Status Codes
		- Easy to Maintain
		- Utilizes HTTP features
	- Cons:
		- Big Payloads
		- Multiple HTTP  roundtrips
	
2) RPC(Remote Procedural Call): Best for APIs exposing  several  actions. (Its all about Actions)
	- RPC  only two methods GET and POST
	- Pros:
		- Easy to understand
		- Lightweight payload
		- High Performance 
	- Cons:
		- Discovery is difficult 
		- Limited standardisations 
		- Leads to function explosion 
3) GraphQL: Best when you need querying  flexibility
	- Client decides the structure  that need from sever , and server produces it.
	- only GET and POST calls.
	- Pros:
		- Saves multiple round trips
		- Avoids versioning
	- Cons:
		- Added Complexity
		- optimising  Performance.
		- Too complicated for a simple API.
----------------------------------------------------------

Event Driven APIs:

1) Web Hooks
	- Example-1 : girlfriend  says I reached home after going to home:
	- Example-2: Paypal recieves notification when friend sends money
	- Example-3 : we no need to call each and every person having a cup of sugar, If some one gives sugar we can collect.
	- It has two main feilds:
		1. Event
		2. Callback URL
	- Pros and Cons:
		- Ensure delivery through retries
		- Apps running  behind firewall can send but receiving  can be tricky.
		- Each webhook represents a single webhook, many events in a short time can be noisy
2) Web sockets
	- client and server perform three way handshake 
	- Bi directional communication.
	- Pros:
		- Bidirectional  low latency communication 
		- reduced overhead of HTTP requests
	- Cons:
		- clients are responsible for communication
		- scalability  challenges
3) HTTP Streaming
	- client sends request
	- server keep on sending data to client
	- Pros:
		- Can stream over simple HTTP
		- Native browser support
	- Cons:
		- Bidirectional  communication  is challenging.
		- Buffering.


Webhook: Trigger the server to send events to pre-defined client endpoints
WebSocket: Bi-directional communication  between client and server
HTTP Streaming: One way communication over HTTP  


--------------------------------------------------------------

1) Authentication : Login
2) Authorisation  : Access Rights ( Normal users dont have permission  to see admin content).



**API Security:**

1) Basic Authentication: 
	- B64 encoded username and password
	- If 3rd party application need perform some operation then user needs to share their credentials  which is a bad idea.
2) OAuth:
	- Allows users to grant access to applications  without having to sharing passwords to them.
3) OpenID Connect
	- Allows clients to verify the identity of end users and get-back profile information  about them
4) Scopes
	- Read and Write scope to individual  scope
5) Refresh Tokens
	- Allow access tokens to be renewed. 

1. OAuth Mechanism:
	- FE to Auth:
		- Redirect URL
		- Response Type 
		- Scope -> Read or Write , openID
	- Auth to FE:
		- Authorisation Code
	- FE to BE
		- Authorisation Code
	-  Auth to BE
		- Access Token
		- ID Token
		- Refresh Token
	- BE to Auth API
		- Access Token 
	