## Development Approach

1.We build open source software. This allows the community to directly review and critique our code and methodologies, and to contribute code for our review. 

2.We use open source technology. We look to build on standard, modern technologies that 
will reduce the operational cost and/or improve the operational performance of models, that 
have solid support options for enterprise use, and that are free for general use. 

3.We are building a full stack development team. Every team member should understand the 
system and technologies, be able to build and test the system and have a working knowledge 
of catastrophe modelling. 

4.We use the community to drive development. We have direct access to many of the leading 
practitioners in the catastrophe modelling domain, and we get practical input through feature 
prioritization, specification and review of working software. 

5.We use partnerships to provide scale, for hosting, support and non-core development. 

## Repository Structure

| **Respository name**	| **Purpose** |
| OasisLMF	| oasislmf Python package, with the core oasis business logic, MDK command line tools and the Oasis API client. |
| OasisPlatform	| Flask application that provides the OasisApi and the Celery worker for running a model. |
| OasisKeysServer	| Flask application for keys services. |
| Ktools	| C++ kernel tools. |
| OasisUI	| Shiny application, Flask app and database for the Flamingo application. |
| Cookiecutter-OasisModel	| Cookiecutter templating for a model implementation. |
| OasisPiWind	| Example model implementation. |

## Build process

TODO
