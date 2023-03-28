## Component architecture

| Rating     | Points | Description                                                                                                                                                                                                                                                                   |
| ---------- | ------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Novice     | 1      | The project does not include well-scoped components. Components have too many responsibilities and overall the application is difficult to follow.                                                                                                                            |
| Developing | 2      | The project includes well-scoped components although they may have a few too many responsibilities. The application relies too heavily on in-class examples that do not solve the particular challenges of the application.                                                   |
| Proficient | 3      | The project includes well-scoped components that only have one or two responsibilities. Presentational components are used regularly and the application is relatively easy to follow. Components reflect the needs and challenges of this application have been implemented. |
| Exemplary  | 4      | The project includes well-scoped components that only have one responsibility. Presentational components are clearly separated and well-defined. The application feels professional and positively complex.                                                                   |

### Example

A _proficient_ score would mean that the project includes a number of sensible and distinct components. For example, the project may include a component that presents a list of items, and each item in that list is its own component.

## Single page applications

| Rating     | Points | Description                                                                                                                                                                                                                                                                                                                                |
| ---------- | ------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Novice     | 1      | The application is structured in such a way where the user must refresh the page to see changes. API calls are not well-controlled and may happen more frequently than needed.                                                                                                                                                             |
| Developing | 2      | The application is responsive to user input and combines many CRUD elements into the same view (eg `new`, `edit` and `delete` are (confusingly) all visible at the same time). Some interactions may be clunky and require a refresh. Alternatively or additionally, API calls are noticeable and clunky.                                  |
| Proficient | 3      | The application feels responsive to user input and combines many CRUD elements in the same view without needing to refresh or redirect. API calls are seamless and happen in the background as needed.                                                                                                                                     |
| Exemplary  | 4      | The application feels responsive to user input and combines many CRUD elements in the same view without needing to refresh or redirect. API calls are seamless and happen in the background as needed. Extra care has been taken to provide a smooth and clear experience for the user, making the app feel more interactive and polished. |

### Example

A _proficient_ score would mean that the project feels like a single page application. For example, it would load information when needed and provide clear responses to the user such as a loading symbol or message. It may also combine multiple CRUD actions into a seamless interface, such as the ability to increase a "like" counter without needing to refresh.
