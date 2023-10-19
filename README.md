# User Agents repository

## Description

A practical datasets containing several user agents. Useful to make web requests and webscraping

The set is composed by:
- a desktop dataset, containing Desktop/Laptop User Agents, such as Windows/Linux/Mac OS and Opera/Safari/Chrome/... browsers
- a mobile dataset, containing Android and iOS User Agents and Safari/Chrome browsers

## Example

It's possibile to integrate the repository within an existing code, simply by downloading the raw file and use it randomly selecting a User Agent. E.g:

```
import random
import requests

return = requests.get('https://raw.githubusercontent.com/AlessandroVaccarino/user-agents/main/agents/desktop.txt')
return_rows = return.text.splitlines()

for _ in range(10):
    user_agent = random.choice(return_rows)
    print(user_agent)
```
