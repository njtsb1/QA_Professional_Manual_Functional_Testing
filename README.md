Daily learning

# The Daily Routine of a QA Professional: The Practice of Manual Functional Testing

Project developed at the GFT Quality Assurance Bootcamp for Women with guidance from specialist [Carolina Santana Louzada](https://github.com/CarolinaSL "Carolina Santana Louzada").

Review useful concepts for manual testing in the agile world, as well as understand and practice activities related to the daily work of a QA, focusing on functional manual testing.

[Diagram](/images/diagram.png)

[LICENSE](/LICENSE)

See [original repository](https://github.com/CarolinaSL/myDioProject).

```Markdown

### Task Workflow

[Task Workflow](/images/Task_Workflow.png)

---

### Bug Workflow

[Bug Workflow](/images/Bug_workflow.png)

---

### User Story 1

**As a user, I want to access the pages: Drivers and Trucks, Images, Videos, and Seasons, and view the available race videos and images, as well as access the details of the ranking tables for each season.**

#### 1. Value
For the system to function properly, it is essential that the user can access links to obtain information about images, videos, tables, drivers, and trucks. The presence of buttons that allow changing languages (pt-BR, en-US, and es-ES) and changing the background color (Dark Mode/Light Mode) is also fundamental.

#### 2. User Narrative
As a customer  
I want to access the Drivers and Trucks, Images, Videos, and Seasons pages  
So I can view and interact with the available information to like, comment, and share.

#### 3. Requirements
- **Actors:** Customer  
- **Platforms:** Web and Web Mobile  
- **Environments:** Pipelines and environments must be created for development, integration testing, acceptance testing, and production  
- **Acceptance Criteria:**  
  - The user does not need to be authenticated to access and interact with the Drivers and Trucks, Images, Videos, and Seasons pages.  
  - The user should see a menu list available to access the links for each item.  
  - The user should see a "Language" button to change the language (pt-BR, en-US, and es-ES).  
  - The user should see a "Dark Mode/Light Mode" button to change the background color of the screen.  

---

### User Story 2

**As a user, I want to access a search bar on any page and perform search operations to return the requested results.**

#### 1. Value
For better usability of the system, it is necessary to include a search bar on the pages to allow a more refined search for the desired items.

#### 2. User Narrative
As a customer  
I want to access a search bar on any page  
So I can search and view the desired items based on the information entered in the bar.

#### 3. Requirements
- **Actors:** Customer  
- **Platforms:** Web and Web Mobile  
- **Environments:** Pipelines and environments must be created for development, integration testing, acceptance testing, and production  
- **Acceptance Criteria:**  
  - The user should see a search bar on any page near the menu list.  
  - The user can enter text in the search bar.  
  - The user should see a clickable button with a magnifying glass icon that executes the search function for the entered text.  
  - The user should see the results returned from their search.  
  - The user should see the message "No results found" if the search does not return any product.  

---

### Mind Map

[Mind Map](/images/Mind_Map.png)

---

### Test Cases (step-by-step)

#### TC 01 (User Story 1)
1. Access the application URL (“https://www.truckracing.com/”)  
2. Access the menu page  
3. Click the "Language" button and choose the language  
4. Click the "Dark Mode/Light Mode" button and change the background color of the screen  
5. Verify that the items listed in the menu appear correctly on the screens  

#### TC 02 (User Story 2)
1. Access the application URL (“https://www.truckracing.com/”)  
2. Access the menu page  
3. Enter text in the search bar  
4. Click the Search button with the magnifying glass icon  
5. Verify that the results show the correct items after the search  

---

### Test Cases (BDD)

#### TC 01 (User Story 1)
Given that the user is on the system’s home screen  
When they access the menu page  
And select an item to check  
And click the "Language" button  
And click the "Dark Mode/Light Mode" button  
Then they verify the language change and the background color change.  

#### TC 02 (User Story 2)
Given that the user is on the system’s home screen  
When they access the menu page  
And enter the text "Seasons" in the search bar  
And click the magnifying glass icon on the "Search" button  
Then they verify the returned result.  

```
