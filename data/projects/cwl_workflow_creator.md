##### Rationale
Technological advances have led to an explosion of information available in digital format across 
most areas of human interest, ranging from individual (e.g. lifestyle choices, personalized health) 
to social concerns (e.g. economics, politics). One major field of research of the incessantly 
growing field of data science is the transformation of _big data_ into a structured form that is 
amenable to manual, assisted or automatic interpretation (e.g. by neural networks and other machine 
learning approaches). Given the enormous variety of possible input data, contexts, research 
questions and tools to address them, processing and (pre-)analysis of data is time consuming. To 
reduce this temporal overhead on a short term, processing and analysis workflows are currently often 
performed _ad hoc_ - but at the cost of severely reduced reusability and reproducibility, thus 
leading to an overall drop in efficiency and quality. By implementing an easy-to-use drag-and-drop 
dependency-aware web application that generates containerized component-based pipelines in a 
standardized workflow language, this project aims to reduce implementation time of both simple and 
complex processing/analysis workflows, while at the same time enforcing "good practices" with regard 
to reusability, reproducibility, sharing and documentation at little to no cost.

##### Approach
The core of the application is the [Common Workflow 
Language](https://github.com/common-workflow-language/common-workflow-language) (CWL), an 
open-source specification for the implementation of component-based workflows, relying on 
[JSON-LD](http://json-ld.org) for describing components and workflows, and 
[Docker](https://www.docker.com/) for providing portable runtime environments.

As the application is supposed to seamlessly integrate with a web-based bioinformatics data analysis 
service currently under development, the application is to be implemented with the following tool 
stack:
- Django: <https://www.djangoproject.com/>
- Django REST framework (back-end): <http://www.django-rest-framework.org/>
- Latest Angular (front-end/GUI): <https://angular.io/>

In particular, a minimal Django app will handle the data models necessary to store and retrieve CWL 
components and save, retrieve and modify the generated CWL workflows. Data models will be serialized 
with the help of the Django REST framework and endpoints defined for a RESTful API. The Angular 
front-end will retrieve components (GET), as well as create (POST), retrieve (GET), modify (UPDATE) 
and visualize workflows (as a network graph on a canvas).

Further details of the Angular implementation will be decided upon together with the student (any 
input is very welcome!), with user experience and performance being the main objectives. However, 
the app should cover the following basic functionality:
- Components can be arranged and re-arranged freely on the canvas via _drag-and-drop_.
- In an overlaid component-based view, default parameters for options, input and output can be 
  set/changed, and relevant information (e.g. an option's help message) easily accessed (e.g. by 
  tooltips).
- New components can be selected/dragged from a sidebar view listing available components.
- Context dependent features, such as handling option dependencies and selectively listing 
  components that are compatible with the currently selected one, are realized by implementing CWL 
  specifications.

##### Challenges
Implementing a reactive, performant and user-friendly stand-alone web application requires 
creativity, as well as rigor with regard to planning and coding. A clean and well documented code 
base is critical to ensure adoption and longevity of the project.

##### Requirements
The ideal student has
- an interest in process automation and creative, user-friendly web design
- experience with a JavaScript front-end framework (ideally Angular2+)
- good working knowledge of Python (Django/REST is a plus)
- basic experience with Git
- read the CWL user guide: <http://www.commonwl.org/v1.0/UserGuide.html>

However, a high level of motivation and an interest to learn about the listed techniques can 
compensate for any lack of experience.
