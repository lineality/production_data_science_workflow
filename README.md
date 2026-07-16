#### production_data_science_workflow

# Navigating Production Data-Science Workflow in Agile Teams
2026.07.15 Geoffrey Gordon Ashbrook


## Novel Aspects of Data-Science Workflow

Cross functional teams and leadership who are accustomed to frontend, backend, and other software engineering (often with standard Agile-like routines) frequently find it difficult to quickly include Data Science into their habitually-familiar norms. 

While both Agile-Software-Development and Data-Science are within STEM more broadly, Data Science projects typically have workflows that differ in important ways from standard front-end or backend work. The goal here is not to go into all the specific steps and details of model-making workflows (those can fit within one broader area below), the goal here is to outline at a higher level some of the 'invisible' unanticipated aspects of Data Science workflow that most often cause preventable issues in workplace projects (and so also could be better covered in educational programs).


#### Data Science projects typically have workflows with the following aspects:

1. The Iceberg-Effect: 
It has long been a consistently accurate rule of thumb for Data-Science (from before deep-learning was popular through into the age of LLM's and generative foundation-models) that the first 90% of work, time, resources is in Dataset creation, exploration, cleaning, 'wrangling' etc. What is described later, and seems to be 'the work' is generally the last 10% or less. This creates an iceberg of data-task-scope that lurks out of sight for project managers, schedulers, and jira ticket creators. Once this hidden 90% of scope is on the radar, it should be that much easier to manage and align on tasks.


2. Task and Case-Specific Details, Steps, and Restrictions:
With 'classification' (vs. 'new discovery') being one example (see: https://github.com/lineality/classification_workflow_datascience), each Data-Science task (such as recommendation, or classification, or prediction) can have specific restrictions, requirements, and required-steps that may not be intuitive based on a common-language summary of the scope (e.g. 'classify this'). Planning time must be allocated and spent to understand this. The person deciding or planning the tasks and schedule will likely need to work with a Data Scientist to make sure that the common-language goals are meaningfully and feasibly translated into well defined Data-Science tasks.


3. Greenfield Production Versions:
Another area where planning-time may be more fundamentally required in data-science compared with other areas of software development is the challenge of wanting to quickly deploy in production Data-Science solutions that currently only exist in Academic or Hobbyist form, not fit or safe for production. In some cases an academic or non-production version may be tantalizingly at hand where there is no known path to a production version. This is predictably frustrating, but it is highly dangerous to push ahead with using something that is not fit for production merely out of impulsiveness and impatience.
As time goes on, more production-oriented data-science tools will be available. But likely long past 2026, a novel Production-Data-Science implementation of a non-production item must be created (or re-created) with care. Sometimes this can be a relatively quick process of re-implementing elements from third party dependencies.
This area also includes tech-stack questions and choices of language, with Python being the dominant language in Data Science, but not always a good choice for production projects. Case by case, language such as Rust should be looked into.


## Hurdles

Some of the main hurdles for adding Data-Science to an existing engineering, frontend, backend or SQL-analytics teams can include:

1. Planning and scheduling steps and deliverables in Jira (or whatever Project Management framework), for example, accounting for the time and resources that are not routine for other software development

2. How to use git and code repositories for data and code (including for general Data Science tools for future use):
Especially in larger organizations, there can be an indefinite 'deer in headlights' set of delays in setting up Data-Science repositories. There are frequently different strong views on how git repositories are set up and used. While the use of repositories for Data Science will not be identical to the use of repositories for Dev-Stage-Prod frontend deployment code (for example), it is important to allocate code sharing and versioning resources to support Data Science tasks.

3. Fumbled planning around third party dependencies: Short Term vs. Long Term
4. The all too common planning-trap may be understandable to anyone by using the 0-60 analogy, as in a car accelerating from 0-60 miles per hour. The analogy is between a project being built to perform everything it needs to do and a car reaching 60-MPH. "Low-Code", "No-Code" tools, various services, and 'third party' software libraries are very common and in some instances may make sense to use. The classic pattern is that using these 'depencies' allows you to accelerate quickly, e.g. going from 0-55 MPH easily. But the catch is that then you end up in a trapped quagmire of technical debt, being unable to ever get from 55 to 60 MPH. 1. The third party system is often not able to fully do everything you need. 2. Your system has been designed and built around this dependency (you are 'locked in'). And 3. There is an ever escalating set of dependency updates, version problems, cross-dependency conflicts, security problems, and on and on. Avoiding 3rd party dependencies takes more planning but is better in the long term. Use of 3rd party dependencies is irresistible in the short term, but with well-known long-term costs and risks.

4. A superficial Agile system that is mostly-kludged-enough to be fine for routine frontend or backend tasks will often be broken by adding the nuanced demands of a Data-Science component. On the other hand a robust Agile-System will be instrumental in getting production Data Science to work.

5. The unfamiliar domain of Data Science tends to make planning around security and performance evaluation insufficient, the incorrect assumption being that these can be safely ignored.

6. "No-news is good-news." A more general perennial problem is a (usually unstated) opposition to data and testing. For whatever reasons, historically there is an overwhelmingly fierce opposition to data and STEM period.

7. Jargon, Terminology, & Lexicons:
Sadly, the quagmire of terminology in Data Science can be a formidable minefield that unavoidably takes time to clearly navigate. There are many terms such as 'model' 'parameter' 'loss' and 'benchmark' that are colliding jargon terms that have different technical definitions in different sub-areas of Data-Science. There are also many common-language terms, such as 'classification' or 'model' or 'explain,' that must be carefully mapped onto the tangled lexicon of Data-Science. If this is not navigated, the project will be a hidden confusion of undefinable word-salad illusions that everyone is interpreting differently and such cannot result in a successful team build. An especially important area here is the 'explainability' or 'auditability' of a system. Both the social requirements and the array of technologies have evolved over time, and the planning and conversation around this cannot be expected to happen quickly and easily. Pressure to punt on this question should be resisted with vigilance.

8. Conceptually the changes involved in including Data-Science workflow into habits for an existing no-data-science set of practices and policies may seem easy, but there is a powerful momentum in the psychology of perception to have the illusion of a flexible, adaptable, generalizable STEM understanding while behavior suggests a rigid and reactionary cargo-cult of unexamined retro-active rationalization of what has been done. 



### Appendix 1:

Also see: https://github.com/lineality/production_datascience_design_areas

