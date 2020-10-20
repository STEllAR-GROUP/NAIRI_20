Data visualization can aid in understanding, especially when little is known about the data or the questions that should be asked of it. Furthermore, visualization can help generate new questions and hypotheses that may not have otherwise been discovered. There are several such scenarios at the intersection of AI and parallelism in this project.

#### Very Large Multi-dimensional Array Visualization

- For algorithm development:
  - Need to understand if therre are structurres within the data that can be leveraged for a more efficient algorithm
- For performance debugging:
  - Need to understand how matrix is distributed and how that distribution correlates with resources and performance
  - Possibly add semi-automaed anomaly detection to assist people in finding points of interest to explore
    -  This can be done with both the matrix visualization and supporting other views.
- Methods: 
  - need to identify what properties of the matrix need to be preserved and communnicated (task analysis, domain analysis) and then develop visual encodings that emphasize these properties
  - need responsive, scalable approach that allows people to navigate large structues quickly


#### Visualizing Performance and Model Behavior in Tandem

- In Situ Model Situational Awareness
  - The asynchronous nature of our proposal allows is ideal for streaming information, allowing both performance and model convergence metrics to be reported while the computation is running
    - There is also potential for steering or stopping iterations early
- Post-run exploration of model & performance as well
  - Prommotes debugging-by-value like in Anteater: https://arxiv.org/abs/1907.02872
    - Note Anteater is heavily limited in scale, we will address scalabililty
