# python-todo

Python console program for managing TODO-tasks.

## Usage (Windows)
1. [Install Python](https://www.python.org/downloads/)
2. Make sure Python is defined on PATH
3. Navigate to folder in CLI
4. $ python todo.py [arguments...]

## Help
- Arguments marked with ? are optional.
- All arguments that triggers a function start with dash(-).
- All arguments must be separated by space only.
- To submit sentences with spaces between words, use quotation marks (", '), otherwise they will be counted as separate arguments.
    - e.g.: $ python todo.py -add "This is a sentence."

---

- ['-tasks', '-t']: prints an indexed list of tasks in the current task list.
- ['-lists', '-l']: prints a list of all task lists.
- ['-add', '-a'] + string: adds the following string to the current task list.
- ['-delete', '-d'] + number: deletes the corresponding task in the current task list.
- ['-check', '-c', '-x'] + number: toggle the completion of the corresponding task in the current task list.
- ['-switch', '-s']+ number + number: switches the position of the two corresponding tasks in the current task list.
- ['-setlist', '-sl']: string: sets the current task list to the string given.
- ['-help', '-h']: prints this information about input arguments.
- ['-test']: runs unit tests and prints the result.

## My Thoughts

I wanted a way to manage some tasks I had to do that sometime repeated daily and the mental list got out of hand. I needed a way to write them down and keep them handy without having to plaster my wall with post-it notes, which is why I thought about making this program. I am aware that there are programs like this out there, as with some of the other projects I have done, but I need some specific functions to help me manage my lists. 

This is not the first time I've made a TODO list, but the previous one is dated and it would be more work and less beneficial rewriting  the old code (PHP). I was unsure what language to choose for this project, but I'm going with Python as I enjoy writing  it and have no need for a online version just yet. I did consider learning Ember or Vue or something similar to cultivate my frontend skills, and might redo this project with that in the future.

## Conclusion

- Better commenting in method
- can be better at catching errors
- try-except overuse? better to let it fail in try-except than if statement? (see addTask filename sanitation before try-except)
- wrapping return messages
- good argument
- testing framework
- less complex methods, distribute tasks to small methods

### TODO:
- check spelling
- groom/trigger reset functions + tests + update help
- write Conclusion

- when printing all lists, add check (0/1 similar to task) to check if all tasks in list are completed
- delete all
- delete all checked tasks
- uncheck all
- rename formatPrintList to formatTasksPrint?
- formatPrintList when empty should return an array of one line: ["The current list (listname) is empty."] or object