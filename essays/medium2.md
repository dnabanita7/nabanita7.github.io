---
layout: essay
type: essay
title: Contributions to Julia during MLH fellowship'20
# All dates must be YYYY-MM-DD format!
date: 2020-08-14
labels:
  - Julia
  - Open Source
  - Major League Hacking
  - GitHub
  - The Startup
---

<img class="ui medium left floated image" src="../images/mlh.png"> **This got published by **The Startup** on Medium.**

I got Julia Summer of Code in May’20. I was excited and started learning about UCX networking and MPI. After 3 weeks, I came to know I was selected for MLH-fellowship’20. I was to contribute to Julia during MLH Fellowship’20. I was in a dilemma as I couldn’t participate in both JSoC and MLH. I continued with both and my first hack week at MLH was somewhat disaster and tiring. I work at Girlscript, Bhubaneswar. Our aim is to conduct programs, sessions and workshops to increase the diversity in tech in and around Bhubaneswar. So, due to that I couldn’t give much time to MLH first hack week project. After that week, I decided to continue with MLH and asked Logan to cut off my name from JSoC list.

During the first week, Gautam Mishra, Biswajit Ghosh and I made Gazel.jl which is an ambient auto brightness tool for laptops/desktops. I created a basic Julia package for gazel. I worked on mapping contrast value to calculate the optimum brightness. I have written the documentation for the project and helped fellow team mates as required.

I contacted Kyle Daruwalla for working on SpikkingNN.jl and told him about my interests in machine learning and deep learning. He said and I quote
```
**Do you prefer working more on the infrastructure or applications side? I have two immediate options that come to mind. We need a MLDatasets.jl and FluxModels.jl to provide a standard way for users to access common ML setups in Flux. Alternatively, we are also looking to establish a benchmark repo that does training and inference for a suite of models and datasets. We would use this repo as a regression test whenever we make changes to Flux or the backend AD tool, Zygote.**
```
I was excited to work on the project. I started reading papers and working on writing vision, RL, language models and training that full range of models. There was always this engineering challenge of integrating everything together too.

I started with AlexNet model, read the paper and it took me a 4 to 5 days to merge it. Well it was easy. Then I started working on ResNet models which took a month to get merged. I read the paper and implemented it. But it had to be more Julian, so we included ``SkipConnection`` layer. It was diffcult at first to understand how SkipConnection works and how to implement it. Kyle helped me and we completely changed the structure of ResNet model.

During this time, I made a feature addition i.e. Adaptive Pooling PR to Flux.jl. @CarloLucibello helped to correct the documentation detailing. @DhairyaLGandhi reviewed and asked for addition of few tests. @avik-pal helped in changing the dispatch of the layers. Adaptive Pooling layers was featured at JuliaCon’20 in the “On the State of Flux | Dhairya Gandhi” at timestamp 14:15.

There was a second hack-week at MLH. This time I worked on fellow-crossing, an office platform inspired by animal crossing game. Kanav Gupta, Stella Wang, Ruby Werman and I partnered up to work on this project. We won a prize at MLH for the best community building project. I worked on wrapping the project using SQLite wrapper and write up a script for using pre-stored database for the office based characters. I had never worked on game-dev or with godot engine before. It was a bit intimidating at the beginning but my team was amazing and we pulled it off.

I also had contacted Paulito Palmes, the maintainer of IBM/AutoMLPipeline.jl. My work was to add a plot feature so that we could use it during pipe-lining other features,scalers, transformers in ML. I have added the plot feature using Makie.jl. I haven’t added tests. I will surely add the tests after the fellowship.

Now, Kyle asked me to add tests so that ResNet and AlexNet model could be tested. I added tests but didn’t know how to check it using Julia. So, he explained how to do testing in general in Julia. I worked on that and my models were merged. @arnold-dev wrote all the vgg models. I added some tests for vgg models and changed vgg.jl and made it work with added tests.

Now, I decided to add the GoogLeNet model. I read the paper and wrote the model. There were some tweaks and all the tests passed and it was merged.

It was bit monotonous to continue working on vision models so I decided to change and start learning Reinforcement Learning. Kyle and I talked with Jun Tian, maintainer of JuliaReinforcementLearning.jl and I started learning RL from David Silver course. Jun guided me to test the existing algorithms in JuliaReinforcementLearning.jl. I learned about ReinforcementLearningBase.jl and ReinforcementLearningCore.jl. It took me two weeks to completely understand RL. During this time, I implemented a Basic DQN in python and tested it. Now, I am reading the paper for Dueling DQN and will implement the same in Julia.

After the fellowship, I will continue working on FluxModels adding more vision models such as InceptionNet v3, v4. I will continue working with Jun on adding more RL models as decided.

Apart from this, I participated in one fun activity i.e. Skribble.io organized by Rasika Karki. It was really fun. I love debating and I participated in one group discussion i.e. “Security and Privacy in AI” organized by Ali Malik. It was interesting.

Micky Chan made us all from pod 0.3.1 as maintainers for JuliaNature which is a compilation of nature inspired algorithms in Julia. Many thanks to Rohan Almeida for helping, being liberal and being a friend as well as a mentor. I had two or three one on one chat with him. He is really humble and always inquisitive about knowing and learning. There is a lot to learn from him.
