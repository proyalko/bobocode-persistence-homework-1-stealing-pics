###Build a Nasa Pictures Stealer

**Create a new web app**
  - Build a stealing command HTTP endpoint
  - Handle a POST request by path ../pictures/steal
  - Request body example { "sol": 14 }
  - Call a corresponding service to trigger stealing pictures
**Implement a Service Layer**
  - Call NASA API and receive pictures data
  - Parse the response to fetch the information about cameras and pictures
  - Store the given data using the persistence layer
**Implement a Persistence Layer**
  - Connect to a local database
  - Create a schema to store the data (please add your SQL scrips to the PR)
    cameras(id, nasa_id, name, created_at)
    pictures(id, nasa_id, img_src, camera_id, created_at)
**Implement a required data access logic that allows storing cameras and pictures**
  - Please note that one camera can have multiple related pictures
  - Make sure you handle data properly so tables do not contain duplicate records
Create a Pull Request (PR) of your solution
Post your insights and a  link to you PR in the thread
Do the "Linked List" Code Review 
Find previous PR and perform a code review
