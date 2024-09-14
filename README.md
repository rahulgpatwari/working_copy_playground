# Working Copy

This is a directory in which I can practice the things I learn by going through the Working Space documentation. This is found [on their webpage](https://workingcopy.app/manual). I'll work on things here and add questions and notes. Then when I'm done I can turn this into a video and put it on YouTube. 

# Chapter One

Create a repository on the github website and then you can download it to the iPad via Working Copy. This is done from the top page by pressing the `+` button and selecting the repository. 

- [] First I need to figure out how I connected Working Copy to my github account. I'm sure there's documentation of that somewhere.
- Create some new files in the remote repository
- Then download them all to the iPad (fetch and merge = pull).

```mermaid
%%{ init: { 'flowchart': { 'curve': 'bump' } } }%%

graph TD


subgraph LOCAL on laptop
  direction LR
  local-files --git add--> staging
  staging --git commit--> local-repository
end

subgraph REMOTE on github.com
  direction LR
  remote-repository
end

local-repository --git push--> remote-repository
remote-repository --git pull--> local-files
```

Some important terms: 

- **commit**: when you create a new file or add changes to an existing one, these are committed to the remote repository (if created remotely). Locally, I think it works a little bit differently. The files are saved, and then can be added to staging. From staging, they can be committed. That way, multiple files (all the files on the stage) can be committed together. These commits are then pushed and pulled back and forth between the remote and local repository as needed.
- **pull**:
- **push**:
- **fetch**:
