# Don't Repeat Yourself  
The DRY principle is stated as Every piece of knowledge must have a single, unambiguous, authoritative representation within a system .    
They apply it quite broadly to include "database schemas, test plans, the build system, even documentation" When the DRY principle is applied successfully, a modification of any single element of a system does not require a change in other logically unrelated elements   
# WET 
The opposing view to DRY is called WET, commonly taken to stand for write everything twice.   
WET solutions are common in multi-tiered architectures where a developer may be tasked with, for example, adding a comment field on a form in a web application.    
# AHA
AHA stands for "avoid hasty abstractions", described by Kent C. Dodds as optimizing for change first,prefer duplication over the wrong abstraction.    
AHA is rooted in the understanding that the deeper the investment we've made into abstracting a piece of software, the more we perceive that the cost of that investment can never be recovered (Sunk cost fallacy).   
# Rule of three 
Rule of three ("Three strikes and you refactor") is a code refactoring rule of thumb to decide when similar pieces of code should be refactored to avoid duplication. It states that two instances of similar code do not require refactoring, but when similar code is used three times, it should be extracted into a new procedure.   

Duplication is considered a bad practice in programming because it makes the code harder to maintain. When the rule encoded in a replicated piece of code changes, whoever maintains the code will have to change it in all places correctly.   

The rule implies that the cost of maintenance certainly outweighs the cost of refactoring and potential bad design when there are three copies, and may or may not if there are only two copies.   
# You aren't gonna need it
You aren't gonna need it (YAGNI) is a principle which arose from extreme programming (XP) that states a programmer should not add functionality until deemed necessary.    
Always implement things when you actually need them, never when you just foresee that you need them. Other forms of the phrase include "You aren't going to need it   
YAGNI is a principle behind the XP practice of "do the simplest thing that could possibly work" (DTSTTCPW). It is meant to be used in combination with several other practices, such as continuous refactoring, continuous automated unit testing, and continuous integration. Used without continuous refactoring.    
# Minimum viable product
A minimum viable product (MVP) is a version of a product with just enough features to be usable by early customers who can then provide feedback for future product development.   
A focus on releasing an MVP means that developers potentially avoid lengthy and (ultimately) unnecessary work. Instead, they iterate on working versions and respond to feedback, challenging and validating assumptions about a product's requirements.   
It is utilized so that prospective entrepreneurs would know whether a given business idea would actually be viable and profitable by testing the assumptions behind a product or business idea.  
The concept can be used to validate a market need for a product and for incremental developments of an existing product.    
An MVP can be part of a strategy and process directed toward making and selling a product to customers. It is a core artifact in an iterative process of idea generation, prototyping, presentation, data collection, analysis and learning.    
Source : [wikipedia](https://en.wikipedia.org/wiki/Main_Page)
