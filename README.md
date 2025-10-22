# Hi, welcome to my Github!

I'm Sergio Rolando Martinez, a web development student, and I'd like to showcase my projects and what I'm currently working on.

## My projects

### [HOOKDB](https://hookdb.sergiorm.dev/)

#### Status
- Progress: 🟩🟩🟩🟩🟩🟩🟩🟩🟩⬜ (90%)
- Work in:
    + 🔧 Fixing minor bugs
    + 📝 Adding new information

#### Introduction
It is a web project focused on video game information and voting, developed by two people. The project took approximately four months to complete in 2024.


My teammate was in charge of the backend. He used:
- Spring: to build the REST API.
- Docker: to set up the containers.
- Hibernate: to connect Spring with MySQL.

In my case, I was responsible for the frontend. I used:
- Figma: to create the design of our website.
- React: used to build the website and create a SPA. This was my first project with React and also the most ambitious I had developed up to that point.
- CSS: to create the styles for the website.
- React Router: a library for efficient page-to-page navigation.
- Toastify: a library for displaying popup notifications.

#### Development
First, I designed the application using Figma, a tool I initially had little experience with. After a couple of days, I became proficient in using it, as its interface and functionality are very similar to Adobe Illustrator, with which I already had experience. You can see it [here](https://www.figma.com/design/8aTidF8pYm4eD3DDD0uoXZ/HOOKDB?node-id=0-1&t=WHkvMr6VvAOC2XFH-1)

Subsequently, I began developing the project structure, divided into the following folders:

- context: stores the provider that allows user information to be managed globally.
- css: global style files shared across different components.
- helpers: .js files that facilitate information handling, such as time calculations and field validations.
- hooks: custom hooks to simplify certain aspects of the project.
- languages: contains translations for static frontend texts.
- modals: windows that appear over the main content, used for example for user registration and login.
- pages: components that represent full screens or routes in your application.
- router: the different routes for navigating through the web application.
- tooltips: small information windows that appear when the user clicks on them.

#### Issues

Numerous problems arose both in the frontend and backend. A key experience mistake on both sides was not standardizing the responses that the backend sent to the frontend. Sometimes it returned an object, an array of objects, or an array of primitive values, which made it difficult to create a robust and simple system for API calls.

During frontend development, a critical issue emerged: when logging in as an administrator and then logging out, a normal user could log in and gain administrator privileges. Initially, I fixed it, and everything seemed to work correctly, but after a week the problem reappeared, occurring consistently every two or three days for two months.

After several failed attempts, I decided to rebuild the entire authentication system from scratch. However, the error persisted, and the real challenge was not just fixing it, but understanding why it seemed temporarily resolved and then failed again.

After an exhaustive investigation with my teammate, we finally discovered the cause: in the Network tab of Google Chrome, there was a disabled button called “Disable cache,” which was affecting the application’s behavior. Previous sessions were being stored in the cache, allowing normal users to temporarily access administrator privileges.

#### Retrospective
In short, we would have liked to include many more features, but time was against us. We had to develop a large number of frontend pages and many backend tables. The things we would have liked to implement are:
- API response standardization: As mentioned earlier in the “Errors” section, each endpoint returned a different response format, which made frontend development much more complicated.
- Testing: Adding testing to our application, although it would require more time, would allow us to automate checks and verify the application without having to do it manually.
- Project structure: While the project has some organization, it leaves much to be desired.
- TypeScript: At that time, I didn’t know TypeScript, so I couldn’t have implemented it. Although it takes more time to apply, in the long run it makes the project more robust.
- More ambitious project: Although the project is ambitious, we had to scale it down due to time constraints and its current size. Many ideas were still left to implement.
- Automation: Currently, adding a game to the database requires a lot of effort from the administrator. We should find a way to obtain game data more easily. Likewise, the interface and available actions are limited and rudimentary, which I believe can be improved.

### [HOOKDB](https://hookdb.sergiorm.dev/)
📊 Progress: 🟩🟩🟩🟩🟩⬜⬜⬜⬜⬜ (50%)

#### Status
- 🚧 Building the web
- 🔧 Fixing minor bugs