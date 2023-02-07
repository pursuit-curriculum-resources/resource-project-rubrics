# Mastery rubric

This section of the project is designed to measure your increasing skill at writing good code and following best practices.

You should aim to score _Proficient_ on all of the criteria listed below. Each rating on the scale, from Developing to Exemplary, is worth 1 point.

## Code quality

| Rating     | Points | Description                                                                                                                                                                                                                                  |
| ---------- | ------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Novice     | 1      | Code infrequently or rarely uses well-named variables, is appropriately indented, or follows best-practices. Code is generally very messy and difficult to understand.                                                                       |
| Developing | 2      | Code uses well-named variables, is appropriately indented, and follows best-practices in some but not all files. Code duplication is sparse. The code is of an acceptable quality for a new developer.                                       |
| Proficient | 3      | Code uses well-named variables, is appropriately indented, and follows best-practices in all files. Code duplication is sparse. The code is of good quality for a new developer and does not contain unnecessary comments or logging.        |
| Exemplary  | 4      | Code uses well-named variables, is appropriately indented, and follows best-practices in all files. Code does not repeat itself. The code quality is representative of a skilled coder and does not contain unnecessary comments or logging. |

### Example

The following code block is an example of _proficient_ or _exemplary_ code. The code is indented correctly, the names are readable, and the comments are brief and helpful. Whether or not the codebase would be considered _exemplary_ would be dependent on the rest of the code.

```javascript
// Initial Fetch for Total Items
fetch(`${rootURL}objects`)
  .then((response) => response.json())
  .then((json) => {
    totalItems = json.total;
    allItemsIds = json.objectIDs;

    // Update look and style
    h2.innerHTML = `Gain access to and explore ${totalItems} artifacts`;
    hiddenAtFirst.forEach((el) => {
      el.classList.remove(`hidden-at-first`);
    });
    document.body.classList.remove(`initial-look`);
    header.classList.add(`new-look`);
  })
  .catch((err) => console.log(err));
```

## Version control history

| Rating     | Points | Description                                                                                                                                                                                     |
| ---------- | ------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Novice     | 1      | The project contains very few commits. Commit messages are generally unhelpful or terse.                                                                                                        |
| Developing | 2      | The project contains a few commits. Commit messages are somewhat descriptive and helpful.                                                                                                       |
| Proficient | 3      | The project contains at least twice as many commits as there are days assigned to the project. Commit messages are descriptive and helpful.                                                     |
| Exemplary  | 4      | The project contains at least twice as many commits as there are days assigned to the project. Commit messages are descriptive and helpful. Each commit only addresses a single bug or feature. |

### Example

The following is an example of a _proficient_ commit history. While there could be more detail added to these commits, the number of commits and general explanation would allow the creator or other developers to see how the project was developed.

```
Total Commits: 15

bug fix
---
create image rotation functionality
---
small fix to about page
---
added media queries for mobile devices
---
completed about page
---
working on about page
---
...
```

## Responsive design

| Rating     | Points | Description                                                                                                                                                                                                                                        |
| ---------- | ------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Novice     | 1      | Little to no effort has been made to create a responsive website. The page is difficult to view and use at certain screen sizes.                                                                                                                   |
| Developing | 2      | The web application is functional on both a desktop and smaller screen. However, pages may have some text that is difficult to read or appears improperly designed depending on the type of screen size.                                           |
| Proficient | 3      | The web application is functional on both a desktop and smaller screen. Pages are readable and navigable, with no content improperly formatted.                                                                                                    |
| Exemplary  | 4      | The web application is functional on both a desktop and a smaller screen. Some elements are changed to make the experience better for users depending on the type of device they are using, such as hamburger menus or conditionally sized images. |

### Example

A _proficient_ web application would be one that makes modest accommodations depending on the screen size. For example, container elements and font size may be adjusted depending on the screen size. The application does not need to be fully redesigned for different screen sizes. An _exemplary_ web application would make specific changes such as the incorporation of hamburger menus or reorganizing entire page layouts.

## Interface functionality

| Rating     | Points | Description                                                                                                                                                                                        |
| ---------- | ------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Novice     | 1      | The application is largely unusable without guidance from the developer.                                                                                                                           |
| Developing | 2      | The large majority of the application works as expected.                                                                                                                                           |
| Proficient | 3      | A user is able to interact with the application with minimal to no obvious errors or mistakes. Any errors that occur display a user-facing message.                                                |
| Exemplary  | 4      | A user is able to interact with the application with no obvious errors or mistakes. Any errors that occur display a helpful user-facing message that is inline with the design of the application. |

### Example

An _exemplary_ web application would look nearly indistinguishable from commonly used websites such as LinkedIn or YouTube. A _proficient_ web application will often the interactions on these websites but may have simple errors that use `alert()`-style messaging or some confusing interactions.
