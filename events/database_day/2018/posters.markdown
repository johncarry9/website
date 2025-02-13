---
layout: page
title: "NWDS Annual Meeting 2018: Posters"
group: "navigation"
id: "database_day_2018"
---

# NWDS Annual Meeting 2018: Posters


* Pei Wang, Simon Fraser University

    Entity resolution is defined as finding different records that refer to the same real-world entity. We study deep entity resolution (DeepER) which aims to find pairs of records that describe the same entity between a local database and a hidden database. The local database can be accessed freely but the hidden database can only be accessed by a keyword-search query interface. To the best of our knowledge, we are the first to study this problem. We first show that straightforward solutions are inefficient because they fail to exploit the ideas of query sharing and local-database-aware crawling. In response, we propose SMARTC RAWL , a novel framework to overcome the limitations. Given a budget of b queries, SMARTCRAWL first constructs a query pool based on the local database and then iteratively issues b queries to the hidden database such that the union of the query results can cover the maximum number of records in the local database. Finally, it performs entity resolution between the local database and the crawled records. We find that query selection is the most challenging aspect, and we investigate how to select the query with the largest benefit at each iteration. SMARTCRAWL seeks to use a hidden database sample to estimate the query benefit. We propose unbiased estimators as well as biased estimators (with small biases) to achieve this goal, and devise efficient algorithms to implement them. We found that (1) biased estimators are much more effective than unbiased estimators, especially when the sample is small (e.g., 0.1%); (2) SMARTCRAWL is more robust to data errors than straightforward solutions. Experimental results over simulated and real hidden databases show that SMARTCRAWL can cover a large portion of the local database with a small budget, outperforming straightforward solutions by a factor of 2 − 7× in a large variety of situations.

* Jinglin Peng, Simon Fraser University

    AQP++: connecting approximate query processing and aggregate precomputation for interactive analytics,"Interactive analytics requires database systems to be able to answer aggregation queries within interactive response times. As theamount of data is continuously growing at an unprecedented rate,this is becoming increasingly challenging. In the past, the database community has proposed twoseparateideas, sampling-based approximate query processing (AQP) and aggregate precomputation(AggPre) such as data cubes, to address this challenge. In this paper, we argue for the need to connect these two separate ideas forinteractive analytics. We propose AQP++, a novel framework to enable the connection. The framework can leverage both a sample as well as a precomputed aggregate to answer user queries.We discuss the advantages of having such a unified framework and identify new challenges to fulfill this vision. We conduct an indepth study of these challenges for range queries and explore both optimaland heuristic solutions to address them. Our experiments using two public benchmarks and one real-world dataset show that AQP++ achieves a more flexible and better trade-off among preprocessing cost, query response time, and answer quality than AQP or AggPre alternatives.

* Brandon Haynes, UW, LightDB: A DBMS for Virtual Reality

    We present the data model and architecture of LightDB, a database management 
system designed to efficiently manage virtual, augmented, and mixed 
reality (VAMR) video content. VAMR video differs from its two-dimensional 
counterpart in that it is spherical with periodic angular dimensions, is 
nonuniformly and continuously sampled, and applications that consume such 
videos often have demanding latency and throughput requirements. To address 
these challenges, LightDB treats VAMR video data as a logically continuous 
six-dimensional light field. Furthermore, LightDB supports a rich set of 
operations over light fields, and automatically transforms queries into 
efficient physical plans. Our design allows developers to declaratively 
express queries over VAMR video data and avoids the need to manually 
optimize workloads. Our LightDB prototype, through experiments with VAMR 
applications from the literature, offers up to 4x throughput improvements 
compared with existing systems in use today.

* Laurel Orr, University of Washington, Probabilistic Database Summarization for Interactive Data Exploration

    Probabilistic Database Summarization for Interactive Data Exploration: We present a probabilistic approach to generate a small, query-able summary of a dataset for interactive data exploration. Departing from traditional summarization techniques, we use the Principle of Maximum Entropy to generate a probabilistic representation of the data that can be used to give approximate query answers. We develop the theoretical framework and formulation of our probabilistic representation and show how to use it to answer queries. We then present solving techniques and give three critical optimizations to improve preprocessing time and query accuracy. Lastly, we experimentally evaluate our work using a 5 GB dataset of flights within the United States and a 210 GB dataset from an astronomy particle simulation. While our current work only supports linear queries, we show that our technique can successfully answer queries faster than sampling while introducing, on average, no more error than sampling and can better distinguish between rare and nonexistent values.

* Tomer Kaftan, University of Washington, Cuttlefish: A Lightweight Primitive for Online Tuning

    Modern data processing applications involve increasingly sophisticated analysis that requires operations beyond traditional relational algebra. As a result, operators in query plans grow in diversity and complexity. Designing query optimizer rules and cost models to automatically pick physical implementations for all of these novel logical operators is impractical. To address this challenge we develop Cuttlefish, a new primitive for tuning query plans online during query execution, which uses multi-armed bandit (MAB) techniques to explore candidate operator implementations and exploit the fastest ones. We prototype Cuttlefish in Apache Spark and tune operators for image convolution, regular expression matching, and relational joins. Our experiments show that Cuttlefish-tuned adaptive convolution and regular expression operators are competitive with an all-knowing oracle that always selects the optimal algorithm, even when individual operator implementations are significantly slower than the optimal. Additionally, Cuttlefish enables join throughput improvements of up to 7.5x over Spark SQL's default query optimizer.

* Basem Elazzabi, Portland State University, SQL Graph & jSQL: A Client-Based Data Analysis Model With Imperative Data Manipulation

    Current data-analysis systems vary from simple and intuitive to powerful and complex. Data-analysis tasks themselves vary from simple tasks, in which a user with little technical knowledge uses a single system or tool, to complex and mind-bending tasks, in which a user programmatically integrates several data-analysis tools. In practice, many data-analysis tasks require integrating multiple systems (client-based and server-based) while the data analysts performing these tasks lack the technical skills to understand or integrate the complex tools, making the analysis task difficult and cumbersome. Further, data analysis tasks often require cooperation from multiple users. Our research introduces a new data-analysis model, which we call SQL graph, that provides a data-analysis environment where data-analysis systems and tools and multiple users can seamlessly collaborate and interact. We also introduce a client-based, imperative data manipulation environment called jSQL that is decoupled from data management systems and is designed to aid data analysis instead of data management.

* Zainab Zolaktaf, UBC, Facilitating data exploration, query composition, and query answer analysis

    In many domains, such as scientific computing, users can directly access and query data  that is stored in large, and often  structured, data sources.   Discovering interesting patterns and efficiently locating relevant information, however, can be challenging. Users  must be aware of the data content and its structure, before they can query it. Furthermore, they have to  interpret the retrieved  results and possibly  refine their query. Essentially, to find information, the user has to engage in a repeated cycle of data exploration, query composition, and  query answer analysis. The focus of my PhD research is on  designing techniques that facilitate  this  interaction.  Specifically, I  examine  the utility of recommender systems for the data exploration and query composition phases, and propose techniques that assist users in the query answer analysis phase. Overall, the solutions developed in my thesis aim to increase the efficiency and decision quality of users.

* Cong Yan, University of Washington, A Comprehensive Study of Performance Inefficiencies in Database-backed Web Applications

    Many modern database-backed web applications are built upon 
Object Relational Mapping (ORM) frameworks. Such frameworks ease
application development by abstracting persistent data as objects,
but usually come with a performance cost. Many applications has very slow
page response when they process increasingly amount of persistent data.
In this work, we studied the source code and bug-tracking systems of 27
open-source popular web applications and analyzed common performance
inefficiencies. We also developed tools to automatically discover these
inefficiencies, and suggested fixes which improves performance from 2x to 39x.
Many fixes can be potentially done automatically.

* Shumo Chu, UW, Cosette: an Automated SQL Prover

    We present Cosette, a solver that can decide the equivalences of SQL queries automatically. Cosette leverages  recent  advances  in  both  automated
constraint solving and interactive theorem proving,  and returns a
counterexample (in terms of input relations) if two queries are not
equivalent, or a proof of equivalence otherwise. Cosette has been used for testing correctness of Apache Calcite, an open source query optimization framework, and building a automated grading tool for data management class in University of Washington.

* Jenny Ortiz, University of Washington, PerfEnforce: A Dynamic Scaling Engine for Analytics with Performance Guarantees

    We present PerfEnforce, a system that enables performance-oriented service level agreements (SLAs) for data analytics. Given a set of tenants and query-level performance SLAs, we address (i) how to dynamically assign compute resources to queries from each tenant, and (ii) how to dynamically resize the multi-tenant service to minimize costs due to compute resources and SLA violation penalties. In a thorough experimental study on our running data analytics service, we show that PerfEnforce reduces total costs of operating the service by up to 40% compared to a static allocation of resources, and that PerfEnforce can meet even strict tenant SLAs with only 4% percent cost overhead compared to a clairvoyant scheduler.

* Jingjing, UW, Delta-Based Neural Network Inference for Fast Video Analytics

* Chris Giossi, Portland State University

    Agile data integration for evaluating the performance of low-cost air quality sensors to monitor traffic-related pollution,"Data analysis often requires using and combining datasets that have different formats, different temporal and spatial granularities or different levels of data quality. Furthermore, data analyses is often done in an exploratory, interactive manner. As the user interactively explores the data, the user may wish to view data at different temporal granularities, in different spatial alignments or with different quality levels. Our agile data integration system aims to support these varying requirements and to do so in an interactive manner making the handling of multiple datasets easier for end users. The user defines an integration specification and the system will respond by temporally and spatially aligning and grouping data according to that specification. As the user explores the data, the desired integration specification may change and our system intends to support such changes using lightweight, agile integration mechanisms. For example, the user may wish to change the granularity at which the data is viewed or move the analysis to a new location. The goal of our agile integration system is to support alternative integrations and fast experimentation. We describe a newly-defined integration specification in the context of scenarios from the integration of transportation and air quality data. We classify how the integration specification and implementation must change to accommodate interactive data exploration in those scenarios.

* Chenglong Wang, University of Washington, Interactive Data Exploration with A SQL Synthesizer

    This demo showcases Scythe, a novel query-by-example
system that can synthesize expressive SQL queries from input output
examples. Scythe is designed to help end-users program
SQL and explore data simply using input-output examples.
From a web-browser, users can obtain SQL queries
with Scythe in an automated, interactive fashion: from a
provided example, Scythe synthesizes SQL queries and resolves
ambiguities via conversations with the users.

* Maaz Ahmad, University of Washington, Casper: Leveraging Big-Data Frameworks Automatically

    Numerous large-scale data processing frameworks have been developed in recent years. To leverage them, however, developers need to familiarize with each framework’s API and painstakingly rewrite existing code. While compilers can be developed to automate such tasks, doing so is often tedious. We present a new tool called Casper that enables sequential programs written in a general-purpose language to leverage large-scale data processing frameworks completely automatically. Rather than syntax-driven translation, Casper first converts the input code to a high-level specification that enables easy translation to the target language. Unlike prior work, Casper uses a novel combination of formal verification and syntax-driven search to effectively prune the space of specifications. In addition, it comes with a novel cost model and runtime monitoring module that selects the optimal implementation given program inputs. We have evaluated Casper by automatically retargeting sequential Java benchmarks to three popular large-scale data processing frameworks: Hadoop, Spark, and Flink. The generated benchmarks perform 17.6× faster on average (and up to 32.2×) as compared to the original, and they are also competitive to the implementations written by domain experts.

* Luis Remis, Intel Labs, Addressing the Dark Side of Vision Research: Storage

    Data access is swiftly becoming a bottleneck in visual data processing, providing an opportunity to influence the way visual data is treated in the storage system. To foster this discussion, we identify two key areas where storage research can strongly influence visual processing run-times: efficient metadata storage and new storage formats for visual data. We propose Visual Data Management System (VDMS), a storage architecture designed for efficient visual data access that exploits next generation hardware and give preliminary results showing how it enables efficient vision analytics.

* Ben McCamish, Oregon State University

    As most database users cannot precisely express their information needs, it is challenging for database querying and exploration interfaces to understand them. We report our progress on developing a novel formal framework for representing and understanding information needs in database querying and exploration. Our framework considers querying as a collaboration between the user and the database system to establish a mutual language for representing information needs. We formalize this collaboration as a signaling game between the user and the data management system. We propose a query answering algorithm and prove that it will improve the effectiveness of answering queries in this environment.

* Lingyang Chu, Simon Fraser University

    Given a large signed social network, how to efficiently find different groups of people that are friendly within the same group and hostile between different groups?

* Walter Cai, UW, Tighter Upper Bounds for Join Cardinality Estimates

    Despite decades of research, modern database systems still struggle with multijoin queries. Users will often experience long wait times occurring with unpredictable frequency detracting from the usabil- ity of the system. In this work we develop a new method to tighten join cardinality upper bounds. The intention for these bounds is to assist the query optimizer (QO) in avoiding expensive physical join plans. Our approach is as follows: leveraging data sketching, and randomized hashing we generate and tighten theoretical join cardinality upper bounds. We outline our base data structures and methodology, and how these bounds may be introduced to a tra- ditional QO framework as a new statistic for physical join plan selection. We evaluate the tightness of our bounds on GooglePlus community graphs and successfully generate degree of magnitude upper bounds even in the presence of multiway cyclic joins.

* Yu Yang, Simon Fraser University

    Imagine we are introducing a new product through a social network, where we know for each user in the network the function of purchase probability with respect to discount. Then, what discount should we offer to those social network users so that, under a predefined budget, the adoption of the product is maximized in expectation?  Although influence maximization has been extensively explored, surprisingly, this appealing practical problem still cannot be answered by the existing influence maximization methods.  In this paper, we tackle the problem systematically. We formulate the general continuous influence maximization problem, investigate the essential properties, and develop a general coordinate descent algorithm as well as the engineering techniques for practical implementation.  Our investigation does not assume any specific influence model and thus is general and principled.  At the same time,  using the most popularly adopted independent influence model as a concrete example, we demonstrate that more efficient methods are feasible under specific influence models.  Our extensive empirical study on four benchmark real world networks with synthesized purchase probability curves clearly illustrates that continuous influence maximization can improve influence spread significantly with very moderate extra running time comparing to the classical influence maximization methods.

* Jose Picado, Oregon State University, Schema Independent Relational Learning

    Learning novel relations from relational databases is an important problem with many applications. Relational learning algorithms learn the definition of a new relation in terms of existing relations in the database. Nevertheless, the same database may be represented under different schemas for various reasons, such as data quality, efficiency and usability. The output of current relational learning algorithms tends to vary quite substantially over the choice of schema. This variation complicates their off-the-shelf application. We introduce and formalize the property of schema independence of relational learning algorithms, and study both the theoretical and empirical dependence of existing algorithms on the common class of (de) composition schema transformations. We show that current algorithms are not schema independent. We propose Castor, a relational learning algorithm that achieves schema independence by leveraging data dependencies.

* Omar Alomeir, UBC, Improving Data Provenance Usability

    Most database provenance work has focused on finding the data that contributed to a query's results and then creating models and semantics to query and generate this provenance information. While comprehensive, Provenance information remains large and overwhelming to users.  Some approaches support limited facilities for visualizing and reporting provenance information; others rely on the user to query and explore the results via different data manipulation languages.

    In this work, we develop a novel provenance system, Pastwatch that uses visualization techniques to make provenance information easier to understand. We provide a case study using Pastwatch on a large, real world, multi-source, financial dataset. Pastwatch tracks the sources and data transformations and presents them in a way that users can understand and trust. We conduct a thorough quantitative user study to show statistically significant results that Pastwatch is more efficient and easier to use than raw provenance data.

* Cyrus Rashtchian, UW CSE / Microsoft Research, Clustering Billions of Reads for DNA Data Storage

    Abstract: Storing data in synthetic DNA offers the possibility of improving information density and durability  by several orders of magnitude compared to current storage technologies. However, DNA data storage requires a computationally intensive process to retrieve the data. In particular, a crucial step in the data retrieval pipeline involves clustering billions of strings with respect to edit distance. Datasets in this domain have many notable properties, such as containing a very large number of small clusters that are well-separated in the edit distance metric space. In this regime, existing algorithms are unsuitable because of either their long running time or low accuracy. To address this issue, we present a novel distributed algorithm for approximately computing the underlying clusters. Our algorithm converges efficiently on any dataset that satisfies certain separability properties, such as those coming from DNA data storage systems. We also prove that, under these assumptions, our algorithm is robust to outliers and high levels of noise. We provide empirical justification of the accuracy, scalability, and convergence of our algorithm on real and synthetic data. Compared to the state-of-the-art algorithm for clustering DNA sequences, our algorithm simultaneously achieves higher accuracy and a 1000x speedup on three real datasets.

    To be presented at NIPS 2017

* Parisa Ataei, Oregon State University 

    Data variations are prevalent in real-world applications. For example, software vendors have to handle numerous variations in the business requirements, conventions, and environmental settings of a software product. In database-backed software, the database of each version may have a different schema and content. As another example, data scientists often need to use a subset of the available databases because using non-relevant information may reduce the effectiveness of the results. Such variations give rise to numerous data variants in these applications. Users often would like to query and/or analyze all such variants simultaneously. For example, a software vendor would like to perform common tests over all versions of its product and a data scientist would like to find the subset of information over which the analytics algorithm delivers the most accurate results. Currently, there is not any systematic and principled approach to managing and querying data variations and users have to use their intuition to perform such analyses. We propose a novel abstraction called a variational database that provides a compact and structured representation of general forms of data variations for relational databases. It hides the variational nature of the data and enables users to express their queries over data variations easily.

* Aly Ahmed, Universtiy of Victoria, Computing source-to-target shortest paths for complex networks in RDBMS

    How do we deal with the exponential growth of complex networks? Are existing algorithms introduced decades ago able to work on big network graphs? In this work, we focus on computing shortest paths (SP) from a source to a target in large network graphs. Main memory algorithms require the graph to fit in memory and they falter when this requirement is not met. We explore SQL-based solutions using a Relational Database Management System (RDBMS). Our approach leverages the intelligent scheduling that a RDBMS performs when executing set-at-a-time expansions of graph vertices, which is in contrast to vertex-at-a-time expansions in classical SP algorithms. Our algorithms perform orders of magnitude faster than baselines and even faster than main memory algorithms for large graphs. Also, we show that our algorithms on RDBMS outperform counterparts running on modern native graph databases, such as Neo4j

* Aliaksei Sandryhaila, Facebook, MyRocks

    MyRocks: the RocksDB storage engine for MySQL

* Srini Iyer, University of Washington, Context-dependent Code Generation from Natural Language

    Existing approaches for automatically mapping natural language (NL) to executable programs in modern general purpose languages, either assume a fixed output structure (generate dynamic parts of a function with a predefined control sequence), a fixed context (generate the body of the same method within a particular class),  or no context at all (generate code tokens synchronously from the textual description). In this paper, we introduce the task of generating source code from NL within the environment specified by a class which consists of all other member variables and methods defined within a class. To learn such a code generator, we use a variant of neural encoder decoder models that (a) encode the NL together with representations for environment identifiers and data types, and (b) decode the resulting code using an attention mechanism with multiple attention heads for each of the NL, the variables and the methods by learning to copy variables and methods. To train our model, we collect and release a new dataset comprising over 100,000 (context, NL, code) tuples, by gathering Java files containing method documentation from public Github repositories. Our model achieves a BLEU score of 29.18 and an exact match accuracy of 8\%, outperforming retrieval and neural sequence to sequence baselines.

* Diana Popova, University of Victoria, Efficient Computation of Importance-Based Communities in Web-Scale Networks Using a Single Machine

    Finding decompositions of a graph into a family of communities is crucial to understanding its underlying structure. Algorithms for finding communities in networks often rely only on structural information and search for cohesive sub-sets of nodes. In practice however, we would like to find communities that are not only cohesive, but also influential or important. In order to capture such communities, Li, Qin, Yu, and Mao introduced a novel community model called ""k-influential community"" based on the concept of k-core, with numerical values representing ""influence"" assigned to the nodes. They formulate the problem of finding the top-r most important communities as finding r connected k-core subgraphs ordered by the lower-bound of their importance. Our goal is to scale-up the computation of top-r, k-core communities to web-scale graphs of tens of billions of edges. We feature several fast new algorithms for this problem. With our implementations, we show that we can efficiently handle massive networks using a single consumer-level machine within a reasonable amount of time.

* Diana Popova, University of Victoria, Efficient Computing of Influence Maximization and Influence Estimation

    Algorithmic problems of computing influence estimation and influence maximization have been extensively studied for decades. We researched several data structures used for the implementation of the Reverse Influence Sampling method proposed by Borgs, Brautbar, Chayes, and Lucier in 2014. Our implementations solve the problems of influence estimation and influence maximization in large graphs faster and using much smaller main memory space than the existing state-of-the-art algorithms while preserving the theoretical guarantee of the approximation that was proven by Borgs et al. for Reverse Influence Sampling.

* Judy Cushing, The Evergreen State College, VISTAS: Visualizing Terrestrial and Aquatic Systems

    Within this NSF-supported research project, computer scientists collaborate closely with environmental scientists and social scientists on a visualization tool to better understand and communicate the environmental science Grand Challenges that span spatial and temporal scales, primarily for geographical areas with complex topography that affects environmental factors. Even as decision stakes rise for policy makers and citizens due to climate impacts, levels of uncertainty increase as global models are downscaled to regions and as forecasts are stretched into an unknowable future. The objective of this project is to address our collaborators’ needs for easy-to-produce visualizations and analytics of their large and complex data sets.  VISTAS currently supports some grid and raster data formats as input, but does not use database technology; it provides the capability for users to write data plug-ins to accommodate new data types.  This poster will discuss current data types input to VISTAS, with the objective of exploring how newor upcoming database technology might be used to improve visualization for a wider variety of users.

* Ben McCamish, Oregon State University, A Game Theoretic Approach to Data Interaction

    As many users cannot precisely express their information needs over databases, database management systems (DBMS) are not able to satisfy their information needs. Current query interfaces generally assume that such users follow a fixed strategy of expressing their information needs, that is, the likelihood by which a user submits a query to express an information need remains unchanged. Using a real-world and large-scale interaction workload, we show that such users learn how to express their information needs in form of queries over the course of several interactions and their learning mechanism is accurately modeled by a reinforcement learning model.  In the light of this finding, we model the interaction between users and DBMS as a game with identical interest between two rational agents whose goal is to establish a common language for representing information needs in form of queries. Built on such a mathematical framework, we propose a reinforcement-based query answering method that leverages users' feedback and prove that it improves the effectiveness of answering queries stochastically speaking and has convergence guarantees. We analyze the challenges of efficient implementation of this method over large-scale relational databases and propose two efficient adaptations of this algorithm over large-scale relational databases. Our extensive empirical studies over real-world query workloads and large-scale relational databases indicate that our algorithms are efficient. Our empirical results also show that our proposed learning mechanism is more effective than the state-of-the-art reinforcement-based query answering method.

* Leilani Battle, University of Washington, Generalizing Behavior-Driven Optimizations for Visual Analytics

    Exploration is a critical phase of the data analysis process, where users (i.e., researchers, analysts and data scientists) aim to make sense of new and unfamiliar datasets, often through the use of a visual analytics system (i.e., Tableau). However as datasets continue to grow rapidly in size and complexity, users struggle to explore their data at interactive speeds. Optimization techniques such as caching and predictive data pre-fetching have shown promise in improving visual exploration performance, however only in limited contexts. In this work, we propose to generalize and extend existing techniques to support large-scale data exploration through common (but sophisticated) visual analytics interfaces. We will present the design of and preliminary findings for an ongoing user study, and provide a high-level overview of our proposed optimization approach.

[Back to the event page](database_day_2018.html)
