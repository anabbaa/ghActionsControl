# ghActionsControl

- add id to the step which hsould refer to then if to the step i want to continue from use context step.id.outcome and to establishyou will compare it with four string success failure cancelled and skipped
- its syntaks add before it any of our function failure() success() cancelled() always() and &&
- also if condition is available on job level
- in cache action it has outputs fiekds which has cache-hit which return true or false
- the difference between if and continue-on-errro the last will continue and will be succeeded
- in conclusion: outcome it checks before error occurs so the conclusion will be success but the outcome is failer in other hand continue-on.error after it occurs the conclusion is always success it may be filed for a technical error or cancelled or skipped

# matrix

- strategy inside it maatrix then write any key its value an array you can add reserved word include or exclude after them

# reusable

- use uses to apply a workflow in another workflow
- the source workflow have a reserved kex input write it by writng its event by indent then insude input theb inide name your input then inide add description type should be string default required should be false in the main workflow use with key word configuration then name of the input then name it
- another thing you can add is serets you use it in the main workflow in differebt way use it by add reserved word secrets with same level of step then inside it your secret variable add to it a value
- you have also output add it in the same level of input inside it add variable as result inide it add describtion and a value then add a step to the job of source workflow name it add ip run a command to establish avariable to save value in it then add in the to level after name of the job inide it a reserved word output inide it a variable and its value context steps.id o a step then .outputs.name of the variable of the command in that step after that in the definition in the over all source work flow add it to the value by context jobs. name of the job which deal with this value .outputs the. name of the variable inside it last step in the main work flow you will add another job directly after job which uses source work flow needs the job which uses the source work flow add a step to it which run command echo with context needs. name of the jobs this job needs to then .output then . name of the variable in the source work flow almost it is result
