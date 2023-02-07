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
