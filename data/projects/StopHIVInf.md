
##### Rationale


Each new HIV infection starts with a virus entering an uninfected host, e.g. through sexual intercourse. Antibodies can bind the incoming virus particles and neutralise them before they can start a new infection. Until now, no vaccine achieved to mount an immune response that confers protective immunity. This was mostly due to antibodies of lesser quality. However, antibodies must also be present in sufficiently high concentrations. Given a mathematical model developed in [our group](http://www.sib.swiss/stadler-tanja/) earlier, one can estimate the antibody concentrations that would be required for reducing the risk of infection below a certain threshold. This information can be used to evaluate a vaccine induced immune response as well as the required concentrations of an antibody based microbicide. The goal of this project is to design an interactive web tool to calculate these levels and make them visually accessible.

![StopHIVInf](data/projects/images/StopHIVInf.jpg)



##### Approach


-	We use the earlier derived mathematical framework for estimating protective antibody levels. This framework has to be adapted for faster computational power.

-	 In a second step, we set up an interactive web application that allows direct visualisation of protective antibody levels.


##### Challenges

- Adaptation of the earlier derived framework requires reprogramming in C or C++. The code available at the moment is relatively slow (written in R).
- Setting up a nice web-based graphical interface.


##### Requirements

- For this project, knowledge in programming in C or C++ as well as basic knowledge of R are desirable. The candidate should not be a complete newbie to web design either. 
