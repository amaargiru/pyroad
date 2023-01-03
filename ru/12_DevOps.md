## Развёртывание и администрирование

Несмотря на то, что темы «git» и особенно «Linux» весьма непросты и объемны, начало кривой обучения у них не очень крутое, поэтому я крайне рекомендую начать освоение DevOps с освоения git'а (хотя бы в объёме add-commit-push, так у вас останется неидеальная, но всё же история изменений) и Linux (в объёме PuTTY + WinSCP, например; скопируйте ваши Python-скрипты через SSH и запустите их на удалённой Linux-машине). На Stepik'е, например, есть прекрасные русскоязычные курсы, подробно объясняющие, кто на ком стоял, а уж сосчитать хорошие англоязычные мануалы по этим тематикам не хватит пальцев у самого распоясавшегося мутанта.  
Поверьте, Linux-консоль, выглядящая на первый взгляд такой непривычной и неудобной, покажется вам гораздо дружелюбнее, когда вы начнете изучать vim. Всё познается в сравнении!  

Что ж, здесь наша карта заканчивается. Попробуйте дойти до последнего зеленого раздела, GitHub Actions; прогоните, например, линтер для своего open source проекта (GitHub Actions бесплатен для проектов с открытым исходным кодом).  

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
