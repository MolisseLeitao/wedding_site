---
title: The Advent of Topology
subtitle: How Topological Data Analysis came to be.
summary: The MNIST dataset is a collection of images of handwritten digits. Before the birth of Convolutional Neural Networks most machine learning approaches arranged each 28x28 pixel image into a 758-dimensional vector. Does this make sense? Does natural data have these coordinates? What if I told you this is seen as standard procedure in "machine learning". Are we cramming vectors, coordinates and metrics where they have no business in?
math: true
diagram: true
reading_time: false  
share: true  
profile: false
weight: 1
commentable: true
image:
  placement: 1
  focal_point: "Center"
  preview_only: false
---

# The Advent of Topology

> "Topology! The stratosphere of human thought! In the twenty-fourth century it might possibly be of use to someone..."
>
> -Aleksandr Solzhenitsyn



### I. An Oncoming PLateau
In August 31st 1955, leading information theorists John McCarthy, Marvin Minsky, Nathaniel, Rochester, and (the father of information theory himself) Claude Shannon proposed the *Dartmouth Summer Research Project on Artificial Intelligence*. Their objective: "That every aspect of learning can be principled so precisely that a machine can be made to simulate it". In other words, to create Artificial Intelligence[^fn1]. 

To say they have failed would be inaccurate. Having witnessed the explosive progress of machine learning at the time, such as the first chess playing program and the self-taught checkers one (\citet{schaeffer1997checkers}) their optimism can't be unjustified. Not much later, disappointment and cynicism led to funding costs and loss of interest in the A.I. field.

In the late 1970s renewed interest fueled new funding and research in the area, prompting the creation the American Association of Artificial Intelligence. In 1984 the **hype** had spiraled out of control and with the funding cutbacks and end of serious research led to the collapse of the A.I. industry in 1987 (\citet{crevier1993ai}).


At the expense of being mediatic, data science has accepted several captivating terms that fuel misconceptions.  Pseudo-scientific terms such as **Big Data** and **Curse of Dimensionality** symbolize existing dilemmas yet are misleading because they push the blame towards the data. When in fact these are symptoms of outdated methodologies. 

**Big Data** conveys the idea that data is volumous, when in fact its our existing methods that can't handle its complexity. **Curse of Dimensionality** misleads one into thinking that high dimensional data behaves abnormally, when it should lead one to question: why care so much about dimensions after all?

The **hype** of past results has created a stubbornness in the methods of Data Analysis. Holding back to previous achievements, existing approaches are not being updated to keep up with the exponential increase in data complexity. The inevitable shortcomings of these same approaches have been blamed on the data (using terms previously discussed) making one believe that our ability for analytical insight is somehow asymptomatic. This inevitably leads to cynicism and loss of interest, so much that there is now talk of a third "A. I. winter". 

This is disheartening since, historically, mathematics has always been ahead of the curve, solving problems years before their applications have been found (such as ellipses).

The restrictions that standard data analysis poses on data (such as assumption of linearity) have not been relaxed from their early insights. Yet what we come to expect from these same models has increased in complexity by orders of magnitude. Predicting the market price of a house versus expecting autonomous driving. There are those who question if the mathematical formalisms of geometry and statistics are sufficient. It might happen that the *nature* of the data  cannot be expressed as a summary of pairwise interactions, in this case geometry which is the study of distance functions, captures only *accidents* on the data. There are many arguments to believe in that insufficiency of purely geometrical methods:

1. **Quantitative characterization is insufficient** The most recurrent problem with big amounts of data is that one doesn't know *what* to look for. Data has knowledge but the way it is presented assumes many forms. As such the first insight must be to extract a robust characterization of the data. For example \citet{carlsson2009topology} presents the example of studying diabetes data. Before developing qualitative insights, the necessary first step is to understand that the disease has 2 very different types.
2. **Metrics are not theoretically justified.** A metric completely governs the behavior of a whole space. It makes no distinction between local and global scopes. Real world scenarios rarely display the same rules, specially when human interactions are involved. More often than not, in areas such as biology or economics, the global structure is defined by a juxtaposition of local behaviors (for example Adam Smith's *Invisible Hand*) and not by pairwise interactions.
3. **Coordinates are not natural.** Although data is *arranged* into vectors it by no means indicates that coordinates make any sense, or that these emerge naturally. The idea that coordinates carry intrinsic meaning is sometimes hindering since it is to be expected that fundamental properties resist coordinate changes. The superior performance of Convolutional Neural Networks (CNNs) can be attributed to this. Before CNNs a $28 \times 28$ pixel image was handled as a vector of $756$ dimensions.
4. **Intrinsic properties should not depend on extrinsic factors.** In geometry a sphere does not exist in of itself, only lying in an Euclidean space. Geometry considers objects always within a bigger space and never as a space of their own. This *extrinsic* view, while more intuitive, is not natural for the object in question, since its *intrinsic* properties are defined depending on the surrounding space that it is laying on. 

### II. The Advent of Topology
Topology is a recent field in Mathematics, it has less than 300 years. It is the study of properties of spaces that are invariant under continuous transformations. Topological methods aim at describing spaces and functions through characterizing features without the concept of distance, therefore spaces with very different geometries can be considered equivalent. Topology surfaced from the necessity of generalizing structural notions such as continuity, compactness and connectedness rigorously. 

Topological Data Analysis (TDA) its the young approach to Data Science through the methods and perspective of Topology. The reasoning is that topological methods directly confront the previously exposed handicaps of present-day methodologies. Below is a brief reasoning why TDA is appropriate to solve each of the points presented above:

1. **Characterization.** Topology was built precisely to study qualitative features of spaces and transformations. Topological Data Analysis extends these methods to points clouds as to extract these very same qualitative properties. Since Topology is a theoretically sound and well structured field, its translation to data analysis generally provides reliable results.
2. **Absence of Metric.** Topology conveys a notion of *nearness* through nested subsets and not through pairwise functions. As such manages to describe robust global identities (shape) through local concepts. This insensitivity to the metric grants topological features an invariance to continuous transformations.
3. **Coordinate free.** Topology only studies properties that do not depend on chosen coordinates. This is due to the fact that Topology considers objects as spaces on their own. In this point of view it is obvious that coordinates make no sense.
4. **Intrinsic point-of-view.** Topology only studies properties that do not depend on chosen coordinates. This is due to the fact that Topology considers objects as spaces on their own. In this point of view it is obvious that coordinates make no sense.

Topological Data Analysis has increasingly gained support in research and traction in its applications. From dimensionality reduction to signal analysis, from graph reconstruction to computer vision. Among many other, it has found widespread success notably on complex network analysis such as neuroscience, contagion network analysis, social networks analysis.





