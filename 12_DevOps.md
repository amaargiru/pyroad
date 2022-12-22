## Deployment and Administration

Despite the fact that git and especially Linux are quite complicated and extensive topics, the beginning of their learning curve isn't very steep, so I highly recommend starting your DevOps mastering with git (at least the add-commit-push part, so you at least have a revision history, flawed as it is) and Linux (PuTTY + WinSCP, for example; copy your Python scripts via SSH and run them on a remote Linux machine). Fortunately, these days good text and video tutorials covering these topics are about as rare as grains of sand on the beach.
Take it from me, the Linux console that looks so strange and inconvenient at first sight will seem much more familiar once you start learning vim. Cognition comes through comparison!

Well, this is where our map ends. Try to reach the last green section, GitHub Actions; run a linter on your open source project, for example (GitHub Actions is free for open source projects).

```mermaid
flowchart TD

subgraph DevOps
direction LR
git -.-> Linux -.-> Development_lifecycle -.-> CI_CD -.-> Containers

subgraph git
direction LR
Basics(Basics)
Branching(Branching)
Tools(Tools)
GitHub(GitHub)
end

subgraph Linux
direction LR
Install(Install)
Directory_Structure("Directory Structure")
Terminal(Terminal)
Input_Output("Input/Output")
bash(bash)
System_administration("System administration")
Network_administration("Network administration")
end

subgraph Development_lifecycle
direction LR
Git_flow("Git-flow")
trunk_based_development("Trunk-based development")
end

subgraph CI_CD
direction LR
Continuous_testing("Continuous testing")
GitHub_Actions("GitHub Actions")
Jenkins(Jenkins)
New_Relic("New Relic")
end

subgraph Containers
direction LR
Docker(Docker)
Kubernetes(Kubernetes)
end

end

classDef trainee fill:#6ADA6A, stroke-width:3px
classDef middle fill:#FF9900, stroke-width:3px

class Basics trainee;
class GitHub trainee;
class Install trainee;
class Directory_Structure trainee;
class Terminal trainee;
class trunk_based_development trainee;
class GitHub_Actions trainee;

class bash middle;
class System_administration middle;
class Network_administration middle;
class Jenkins middle;
class New_Relic middle;
class Docker middle;
class Kubernetes middle;
```
