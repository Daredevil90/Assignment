# Steps for Setup of Project
1) Use the sample env in the public directory located in both Frontend and Backend
2) FIll the env variables with required values and place them in the root directory
3) run `npm i` then  `npm run dev` on both Frontend and Backend
## Hasura PostgreSQL Table Schema Structure
 def users{<br/> 
 column 1:id uuid primary key <br/> 
 column 2:name text <br/> 
 column 3:email text <br/> 
 column 4:password text <br/> 
 column 5:created_at(suggested by Hasura) <br/> 
 column 6:updated_at(suggested by Hasura) <br/> 
 column 7:balance numeric  <br/> 
 column 8:access_token text <br/> 
 }
 ## Design Decisions
 1) Assumption 1: Decided to use a dummy system to substitute for real beneficiaries or bank accounts and thus provide no way to link such accounts
 2) Assumption 2: Since banks or beneficiaries are not linked  it makes no sense to implement a withdrawal and deposit transactions for the user to perform on itself
3) Assumption 3: The Net Banking function uses names of other users on the platform, there are better ways to implement this but because of time requirements I did not spend much time on designing the backend schemas to accomodate them.

