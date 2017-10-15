# Universal ICO contract 
This is a universal ICO contract what you could use as is or start development based on it.

## How to setup development environment and run tests?

1. Install `docker` if you don't have it.
1. Clone this repo.
1. Run `docker-compose build --no-cache`.
1. Run `docker-compose up -d`. 
You should wait a bit until Oraclize ethereum-bridge initialize. Wait for 
`Please add this line to your contract constructor:
OAR = OraclizeAddrResolverI(0x6f485C8BF6fc43eA212E93BBF8ce046C7f1cb475);`
message to appear. To check for it run `docker logs ico_oracle_1`.
1. Install dependencies: `docker-compose exec workspace yarn`.
1. To run tests: `docker-compose exec workspace truffle test`.