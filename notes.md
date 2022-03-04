Decoupled Approach

  - Mystery user makes auth request to passport, returned to client as identified user.
    - Once within the site/authenticated, subsequent requests run through GraphQL using the identified users id
  
- This approach does not involve using any mutations

Coupled Approach
  - Mystery User send auth request/mutation to GraphQL, who passes it off to PassPort
    - Passport adds cookie/returns data for identified user to GraphQL -> to client
    - Subseuent requests run through GraphQL

Planned Mutations for Auth App

Types: User

Mutations: Signup, Login, Logout
