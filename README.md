# Running the Application
---
## Requirements
***
* ####  Flask
* ####  Virtual Environment

## Setup
***
#### [Flask and Virtual Environment Setup](http://flask.pocoo.org/docs/0.11/installation/)

##### After pulling the project

#### Windows
> C:\path\to\your\project> &lt;name of your virtual environment>\Scripts\activate

> C:\path\to\your\project> set FLASK_APP=app.py

> C:\path\to\your\project> python -m flask run

#### Linux
> $: export FLASK_APP=hello.py

> $: flask run

## Contributions
***
##### Before making changes to your project create a branch with your name:

> $: git branch &lt;your name>

> $: git checkout &lt;your name>

##### After making your changes

> $: git add -A

> $: git commit -m "Your Commit Message"

> $: git push origin &lt;your name>


## Additional Information

#### Website Requirements
- Post Questions to a forum
- Create a profile
- Login functionality
- Update profile (Along with Resume)
- View another members profile
- Make posts to their pages (like a blog)
- Showcase projects (i.e Upload Projects)
- Forums will have predefined threads
    * Admins able to manage threads
- Main page to contain news and announcements
    * May use external APIs to pull news as well as allow certain members to post news
- Sign up functionality
    * Generate a number each week users need to enter this number to sign up
- Allow members to check-in to a meeting
- Search by
    * Member
    * Project
    * News
    * All

#### Entities Outlined
- Post
    * topic : String
    * content : String
    * created : DateTime
    * createdBy : User
    * comments : ArrayList<Comment>
- UserPost extends Post
    * thread : Thread
- Thread extends Post
    * permissions : ArrayList<String> (may need to change)
- NewsPost extends Post
    * link : String
- User
    * firstname : String
    * lastname : String
    * created : DateTime
    * dob : DateTime (make final)
    * alias : String
    * description: String
    * profilePicture : String
- Project
    * sourceLink : String
    * title : String
    * description : String
    * contributors : ArrayList<User>
- Comment
    * createdBy : User
    * content : String
    * replies : ArrayList<Comment>



## Happy Coding!!
