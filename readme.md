<h1 align="center">Explately</h1>

<!-- ### Use Case Diagram -->

<!-- - **Member:** All members can search for other members, companies or jobs, as well as send requests for connection, create posts, etc.
- **Admin:** Mainly responsible for admin functions such as blocking and unblocking a member, etc.
- **System:** Mainly responsible for sending notifications for new messages, connections invites, etc. -->

<!-- Here are the top use cases of our system: -->

<!-- - **Add/update profile:** Any member should be able to create their profile to reflect their experiences, education, skills, and accomplishments.
- **Search:** Members can search other members, companies or jobs. Members can send a connection request to other members.
- **Follow or Unfollow member or company:** Any member can follow or unfollow any other member or a company.
- **Send message:** Any member can send a message to any of their connections.
- **Create post:** Any member can create a post to share with their connections, as well as like other posts or add comments to any post.
- **Send notifications:** The system will be able to send notifications for new messages, connection invites, etc. -->

<!-- <p align="center">
    <img src="/media/linkedin-use-case-diagram.svg" alt="Use Case Diagram">
</p> -->

<p align="center">
    <img src="/media/uml.svg" alt="UML">
</p>

### Class Diagram

<p>
    <img src="/media/er.svg" alt="Class Diagram">
</p>

# **Flow:**
## [Flow Document Link](https://docs.google.com/document/d/1y1g0VjbBMSH0HbBKWvRKNXpzJzeJjsLi-LzBt_YqMfM/edit?usp=sharing)


**Google OAuth:** Google OAuth integration.

- Provide the user with a link to the authentication system that includes what data you’d like the user to give your application access to (scopes), your client ID, and a redirect URL
- When the user clicks the link and grants access to your application, they will be redirected back to your application with a security code in the query string
- The security code is sent to your application’s server
- Your application’s server uses the security code, client ID, and client secret to request an access token & bearer token
- The access token and bearer token are used to fetch the user’s profile information on their behalf
- The profile information can be used to either verify them against an existing user in your system or create a new user
- You finally issue the user a token that will work with authentication system(JWT).

<p align="center">
    <img src="/media/google-login.webp" alt="login Activity Diagram">
    <br />
    Diagram for login with Google OAuth.
</p>



<!-- ### Activity Diagrams

**Authentication && Authorization:** Register && Login user with Json Web Token(JWT).

**Register New User:**

<p align="center">
    <img src="/media/register.svg" alt="register Activity Diagram">
    <br />
    Activity Diagram for register new user.
</p>

**Login User:**

<p align="center">
    <img src="/media/login.svg" alt="login Activity Diagram">
    <br />
    Activity Diagram for login user.
</p>

**Send message:** Any Member can perform this activity. After sending a message, the system needs to send a notification to all the requested members. Here are the steps for sending a message:

<p align="center">
    <img src="/media/sendmsg.svg" alt="LinkedIn Send Message Activity Diagram">
    <br />
    Activity Diagram for Send Message
</p>

**Add experience to profile:** Any LinkedIn member can perform this activity. Here are the steps to add experience to a member profile:

<p align="center">
   <img src="/media/exp.svg" alt="LinkedIn Send Message Activity Diagram">
    <br />
    Activity Diagram for Add Experience to Profile.
</p>

Start
Receive a new CV/resume
Parse the CV/resume to extract relevant information (e.g., candidate's name, contact information, work experience, education, skills, etc.)
Store the extracted information in a database or other storage system
Index the information for fast retrieval
Allow recruiters or hiring managers to search the database for candidates who match specific criteria (e.g., job title, location, experience, education, etc.)
Display a list of matching candidates
Allow recruiters or hiring managers to view the full CV/resume of selected candidates
Allow recruiters or hiring managers to contact selected candidates for further screening or interviews
End

The user creates an account on the CV bank platform.
The user uploads their CV or creates a new one using the platform's CV builder.
The user can edit, update or delete their CV anytime.
Recruiters or potential employers can search for candidates using various filters, such as job title, experience, skills, and location.
The platform displays a list of relevant CVs for the job posting.
Recruiters can view the candidate's profile, work experience, education, skills, and contact details.
The recruiter can shortlist or reject the candidate.
The candidate receives a notification if they are shortlisted, and the recruiter contacts them for further discussions.
The platform sends alerts to candidates for job openings based on their skills and experience.
The platform provides analytics on CV views, job applications, and candidate feedback. -->
