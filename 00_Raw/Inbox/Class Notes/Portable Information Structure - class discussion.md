## Week 1, Session 1 Class Notes
The class began with introductions. Students shared their program track, areas of specialization, and one recent creative activity. The class included students from different MSIM tracks and one MLIS student. Creative activities mentioned included pottery, crochet, rock climbing, piano, wig styling, photography, writing, painting, cooking, decorating office space, building a media server, and working on a wearable device that translates movement into music. This gave a sense that the class includes people with different backgrounds and interests, which may shape the kinds of projects they choose later.

The instructor then explained the general purpose of the course. The course is about portable information structures and how to recognize, analyze, design, and implement them. He said the title itself requires work to understand because students need to think about portability, information, and structure together. The class will include both theory and implementation. Students can choose how deeply they want to go into building things. Some may focus more on design, while others may want to implement more advanced systems. The instructor emphasized that building and trying things is an important way to learn, even if what is built is simple.

A story from the instructor’s startup experience helped explain why this class matters. He described building a data product and choosing a JSON-based format because he believed it was the best design for customers. However, the CEO wanted CSV files instead because he was more familiar with them and wanted to open and inspect the data easily. The instructor’s design ended up working for the customer, but the situation still created conflict. The lesson was that in information management there may be multiple valid solutions, and being technically right is not always enough. Human factors, collaboration, and the actual needs of users and stakeholders matter. A person can be right and still lose if they do not handle those dynamics well.

The instructor then reviewed the syllabus and course structure. He said Canvas is the main place for the course. The schedule is on the home page, and the syllabus is another important reference. The course is not organized mainly through modules, so students should rely on the schedule page and assignment pages. He also explained that the class includes discussion, reading, individual and group activities, and short presentations. The course is designed around being in class, participating, trying things, and asking for help when needed. He said that the students who do best are usually the ones who ask for help when they get stuck.

The grading breakdown was also covered. The class includes individual assignments, a group project, in-class group work, class notes, and project feedback. The instructor described the course as highly structured in schedule, but flexible in policy. He has a flexible extension policy: if a student needs more time, they only need to ask before the deadline and propose a new deadline. No explanation is required. The main goal is learning, not punishing students for deadlines.

The instructor also discussed the assignment pattern. In general, Mondays are group-related and Wednesdays are individual-related. Group assignments are labeled G, and individual assignments are labeled I. There are many small assignments rather than a few large ones. Each assignment has a required file type, and Canvas will restrict submissions to that file type. The instructor said this is meant to help students gain familiarity with different information structures and formats such as Markdown, JSON, and others. He also said that there will be lab-style class time to help students set up tools and complete assignments, and that students should not assume something is too difficult before trying it.

A major part of class was the overview of the final project. The final project is cumulative and draws on work from the smaller assignments. Students will identify an existing information structure “in the wild” that they care about and want to improve. They can focus on different kinds of outcomes, such as better visualization, better analysis, prediction, or automation. The project framework is based on a Six Sigma style process: identify or ideate, define, analyze, improve, and control. The instructor said the group project deliverables will include a GitHub repository and a README, and that students will work with several file types across the quarter. The project can connect to a student’s own interests, specialty, or career goals.

The instructor also addressed generative AI. He said it cannot realistically be policed, but students should avoid what he called “cognitive surrender,” meaning using AI just to get something done without engaging with the work. He gave an example of receiving an AI-generated proposal that looked careless and unprofessional. His point was that overreliance on AI can lead to low-quality work and a loss of attention to detail. He encouraged students to notice when that is happening and instead ask for more time or step back and do the work more intentionally.  

The class finished with work on the first individual assignment, I0, which involved drafting a CV-style entry. The purpose was not necessarily to literally put this class on a resume, but to think clearly about what success in the class would look like. The instructor connected this to the idea that “everything is created twice”: first in thought, then in action. Students were asked to think about what they would want to be able to say to a future employer or manager about what they achieved. The suggested structure was to identify a problem, explain what they contributed, and explain the outcome. Students then worked individually, shared with a partner, and discussed ideas. One student shared that they wanted to build confidence in approaching unfamiliar information systems, and the instructor said that was a strong goal for the course.

At the end, there was also clarification about the class notes assignment. The student assigned to capture notes should submit them in the required format and also post them in the class discussion thread with the correct week and session label. This is only required for the student assigned to that class session.


## Week 1, Session 2 Class Notes
**Information structure: why learn?**
- you can't disengage portable information structures from their linguistic roots
- Make assumptions on the relation of labels in a document (e.g. a CSV with headers name, cx, date)

Data structures are a form of information structure - often codifying labels into familiar/intuitive forms

**Information structures (Wikipedia)**

Consist of three main notions:

- focus: contributing new, non-derivative, or contrastive information; updates the model; tells someone information that isn't obviously known based on the other words/information being delivered
- givenness: common related information that is already familiar to the audience; this includes information that has been previously discussed that is now being recovered
- topic: what is being talked about

These notions are inherently understood and communicated during conversation - easy to tell when they are missing

Learning and recognizing these in different contexts is crucial to understanding what is being discussed

The meaning of sentences can change, based on how these notions are positioned

- learning new languages: the differences in grammar, sentence structure, etc. can make even familiar phrases more difficult
- Writing style used in Oxford article: very academic, very dense, difficult to parse even though we can all read English

**Why is structured data important from a legal context?**

Structured data: in a formal schema, such as in a database; quantitative (values, metrics)

Unstructured data: emails, memos; qualitative (more descriptive); can also contain docs (emails/texts), images, video, audio

Metadata: data about data; helps contextualize the data; really useful for searching for/looking up the data from other contexts as well

Using our email example, could involve data such as who sent it, to whom, at what time, etc.

In legal proceedings/discovering, mainly holding unstructured data can lead to unintended or unwanted outcomes

Structured data allows one to more easily identify and point to areas of importance without potentially revealing something harmful

For businesses, having more structured data allows them to draw stronger insights from easily accessible locations

Types of metadata:

- entity relationships
- data dictionaries
- lineage mapping
- schema and layouts

**JSON**

JSON (Javascript Object Notation) is a method to represent data as Javascript objects. These objects are similar to dictionaries in Python or other languages, and consist of storing data in key (identifier) and value pairs

These objects support nesting other Javascript data types such as lists ([ ]), and even other objects

Key: "name"; value: "steve"

Can infer attributes of key values. Keys must be strings.

'''["record1": { "name": "steve", "id": 12345 }, "record2": {"date": "4/1/2026"}]'''

This JSON contains a list of dictionaries, and each dictionary has its own nested dictionary

The good: recognizing there are two different records stored, and thus they must be distinct, so they are structured properly

The bad: the records do not contain the same information; labeling them record1, record2 does not convey information about what they are, the outer dictionaries are invalid syntax

**Information system examples**

Bus route: "KC Transportation Routes", "Inform riders about the bus schedule information", "Website, API call, bus stop, navigation app", "HTML - tables, if viewed via a website (portable, derivative)", "datetime or string"

## Week 2, Session 1 Class Notes
### Class Session Summary: Access to Information & Information Structures

1. Framing the Session

- The class focused on access to information, not just as a technical issue but as a social, ethical, political, and structural concern
- Two assigned articles presented overlapping but distinct perspectives on information access
- Emphasis was placed on portable, large‑scale information structures and how access affects society at multiple levels

2. Existing Beliefs About the Right to Access Information

- The instructor prompted students to reflect on prior beliefs about:

- Who has the right to access information
- When access is beneficial vs. harmful

- Students referenced prior coursework and foundational figures in information ethics

3. Open Source Software

- Richard Stallman was discussed as a key figure in the open-source and free software movement
- Core arguments for free/open software:

- Software becomes a fundamental infrastructure for modern society
- Broad societal benefits when software is open:

- Individuals, businesses, consumers, and suppliers all benefit
- Encourages competition, innovation, and collaboration
- Allows people to build upon and improve others’ work
- Enables smaller companies to innovate instead of being blocked by proprietary systems

- Charging for access was framed as rent‑seeking behavior that extracts value without adding societal benefit

4. Tension: Open Access vs. Restricted Knowledge

- Not all information should necessarily be open:

- Certain types of information are sacred, culturally sensitive, or potentially harmful

- Example discussed:

- Indigenous knowledge and land use in the Grand Canyon
- Authors intentionally obscured or misdirected location information to:

- Protect culturally significant sites
- Prevent tourism and physical harm

- This highlighted an ongoing ethical tension:

- The democratic value of access
- vs. the responsibility to protect communities and cultural practices

5. Access to Information for Democracy & Accountability

- Access to information is crucial for:

- Government accountability
- Public health
- Environmental protection

- Cited examples:

- Air quality data in London

- Poor transparency contributed to children’s health issues
- Public access enabled accountability and reform

- Flint, Michigan water crisis

- Lead contamination was known, but the severity was not transparently communicated
- Lack of accessible, understandable information delayed action

6. Environmental Harm & Corporate Responsibility

- Corporations may resist transparency due to:

- Legal liability
- Accountability for pollution or harm

- Instructor shared professional experience:

- GE involved in environmental mitigation efforts from own upstream impacts
- Reinforced the idea that information access directly impacts environmental justice

7. How Information Should Be Provided to Improve Access

- Information access is not just _availability_, but usability
- Best practices discussed:

- Provide data in multiple formats
- Prefer open, non‑proprietary formats

- Examples from data.gov:

- Structured formats: CSV, RDF, JSON, XML
- Unstructured formats: PDFs, HTML, TIFF
- APIs allow programmatic access

- Key distinctions:

- Structured data is ideal for analysis and reuse
- Unstructured data is often better presented via web pages
- Systems should offer multiple access paths

8. Libraries, Preservation, and Physical Access

- Federal Depository Libraries:

- Preserve government information
- Provide free, physical access to the public
- Ensure long‑term preservation and equity of access

- Although many materials are now digital:

- Libraries remain essential for people without personal technology or reliable internet

9. FOIA (Freedom of Information Act)

- FOIA requests allow public access to federal information
- Examples:

- FBI / CIA reading rooms

- Limitations of FOIA access:

- Often delivered as:

- Zipped files
- Scanned documents
- Heavily redacted materials

- Technically “available,” but not meaningfully accessible or usable

- Demonstrates difference between theoretical access and practical access

10. Access Includes File Size and Technical Constraints

- Accessibility is affected by:

- File size
- Storage requirements
- Hardware limitations

- Example:

- A 500MB class file caused student devices to crash

- Key takeaway:

- Information must be sized and structured so the average person can open, store, and work with it

11. Government Obligation to Publish Information

- Governments have a proactive responsibility to publish information
- This is a civic expectation tied to:

- Taxpayer funding
- Democratic accountability

- Many people feel disconnected from civic information:

- Information technically exists, but is difficult to find or understand
- Tax information used as a primary example

12. Tax Information as a Case Study in Opacity

- Tax code issues:

- Highly complex and inaccessible to non‑experts
- Entire industries (e.g., tax preparation) benefit from this complexity

- “Gray areas” in tax law:

- Accountants understand audit thresholds and risk modeling
- Ordinary taxpayers do not have access to this critical information

- IRS audit process:

- Based on actuarial risk models
- Not fully transparent because:

- It could enable tax evasion
- Resources are limited
- Enforcement strategies would be undermined

13. Information, Objectivity, and Power in Organizations

- Performance reviews used as an analogy:

- Often portrayed as objective through numbers and scores
- In reality:

- Decisions are human and subjective
- Data is frequently created _after_ decisions to justify them

- Information can:

- Create a sense of fairness
- Mask subjective or political decision‑making

- Raises questions about:

- Transparency
- What information should be accessible to employees and citizens
- Sensitivity vs. accountability

14. In‑Class Exercise: Information Stories

- Students created “information stories” using a template:

- As a (person / citizen / business)
- I need access to (specific information)
- So that I can (achieve a goal)

- Example user stories:

- Community member → public transportation info → mobility
- Citizen → school funding info → transparency and budgeting awareness
- Individual → benefits/social security info → claim rights

15. Group Project (G2) Introduction

- Goal:

- Generate at least three project ideas

- “Product” defined as:

- An information structure, not a physical or commercial product

- Project requirements:

- Summary of the information source
- What it enables
- Optional link to specialization

- Encouragement to:

- Move beyond purely personal interests
- Choose projects with broader societal relevance
- Focus on improving access, structure, portability, and transparency

## Week 2, Session 2 Class Notes
#### **Introduction & Framing**

The class began by framing portability as something that is **not fully defined**, especially when applied to information structures. While we often think of portability in terms of moving data, the discussion pushed us to think more critically about what it actually means for data to move **with meaning, usability, and context intact**.

The session was split into two parts:

- First half focused on readings and discussion
- Second half focused on applying these ideas through the I2 assignment

A key goal was to **develop a working definition of portability for information structures**, recognizing that this definition may evolve as we build and test systems.

#### **Understanding Data Portability**

From the readings (Chapter 2 & 4 and Wikipedia), data portability is not just about movement, but about **rights, access, and system design decisions**.

Some core ideas that came up:

- The **right to transfer personal data**
- Being able to **access data without needing to claim ownership**
- Avoiding **vendor lock-in**, where systems trap user data

At a surface level, portability seems simple, but the discussion revealed that it introduces deeper questions about:

- Who controls data
- How data is interpreted across systems
- What gets lost (or protected) in the transfer

#### **What We Mean by “Data Portability”**

One way to think about data portability is as a **feature of a system** that allows users to move their data elsewhere. However, this definition is incomplete without considering the tradeoffs.

From discussion:

- It enables users to **download and reuse their data easily**
- It supports **interoperability across systems**
- It can help **increase competition** by reducing dependency on platforms

At the same time:

- It raises **privacy and security concerns**
- It does not automatically guarantee meaningful reuse

This led to an important realization:  
**Just because data is portable does not mean it is usable.**

#### **Key Themes from Readings**

Two major themes stood out and were repeatedly referenced in discussion:

- **Competition**
    - Lack of portability can limit competition
    - Portability enables users to move between platforms more freely
- **Standards**
    - Portability depends heavily on shared formats and standards
    - Without standardization, data may technically move but still be unusable

#### **Developing a Definition of Portable Information Structures (PIS)**

In small groups, we worked toward defining what makes an information structure “portable.” Across discussions, a few consistent ideas emerged.

At a high level, portable information structures are not just about moving data, but about ensuring that data remains:

- **Understandable**
- **Interpretable**
- **Reusable across contexts**

#### **Key Characteristics of Portable Information Structures**

#### 1. Interoperability and Reusability

Portable structures should allow data to move between systems **without requiring major transformation or re-collection**.

- Data should work across platforms
- Formats like CSV and JSON make this easier
- APIs and tools (readers, transformers) often support this process

There was also an emphasis that portability is not just technical, but **ecosystem-driven**. Systems, tools, and formats all need to work together.

#### 2. Preservation of Meaning

A major point from discussion was that portability is not just about access, but about **retaining meaning**.

- Data should not lose its **interpretability** when moved
- The receiving system should understand what the data represents
- This connects to the idea of **semantic integrity**

Some groups described this as data being “complete on its own” or able to **explain itself without additional context**.

#### 3. Role of Metadata and Self-Descriptiveness

Metadata came up as a critical component of portability.

- Data includes both **values and metadata**
- Metadata helps explain:
    - Purpose
    - Ownership
    - Structure
- It creates **shared semantics**, making data easier to interpret

There was also an interesting point that sometimes **sharing metadata (instead of raw data)** can improve portability while still protecting sensitive information.

#### 4. Accessibility and Usability

Access is not just about making data available, but making it **usable**.

- Data should be understandable by both **humans and machines**
- Structures should not require excessive effort to interpret
- Accessibility introduces concerns around:
    - Privacy
    - Security
    - Misuse

This reinforced that **access and portability are closely linked but not identical**.

#### 5. Privacy and Security Tension

A recurring theme was the **natural tension between portability and privacy/security**.

- More portability can mean more exposure
- Systems need ways to:
    - Remove sensitive data
    - Control what is shared

Some groups noted that privacy and security may not always be part of the _definition_, but they are always part of the _design considerations_.

#### **Key Tension Identified**

Across all discussions, one core tension stood out:

- Transparency and openness vs protection of sensitive data
- Ease of transfer vs risk of misuse
- Interoperability vs system-specific constraints

This tension is central to designing portable information structures.

#### **I2 Assignment: Connecting Portability to Integration**

The second half of class focused on applying these ideas through the I2 assignment.

The goal is to understand how **data integration builds on portability**.  
Portability makes movement possible, while integration makes data **work together**.

#### **Assignment Approach**

You have flexibility in how you approach it:

- You can use Gen AI and go more advanced
- Or follow the provided example and modify it

Important note:

- Your data does NOT need to start as JSON
- But the final output should be **JSON or CSV**
- Tools like BeautifulSoup can help extract and convert data

#### **Tips for Getting Started**

A helpful way to approach the assignment is to start with something you’re genuinely interested in.

- Find a dataset
- Identify a field that can connect to another dataset
- Add value through integration

Example:

- Book dataset
- Use genre field
- Pull genre definitions from Wikipedia
- Add a new column with definitions

#### **Example Data Sources**

- **Data.gov** has a lot of high-quality public datasets across different domains like healthcare, transportation, and government data
- **Seattle Public Libraries** provides good public data, especially around books, borrowing patterns, and catalog information
- **Kaggle** is a great resource for a wide range of public datasets, including cleaned and ready-to-use datasets for analysis

#### **Logistics**

- Groups on Canvas will be made editable by the professor, so if you want to work in a group, you should create your group there.  
      
    AI was used to organize raw notes into a clearer, more structured format for readability.

## Week 3, Session 1 Class Notes
Intro to class:

- Professor worked on a knowledge graph team, and we can incorporate knowledge graphs into our final project if we want
- Continue working on definitions of information structures from last week
- Do data normalization, data coding – want to come out with a consolidated definition, which will involve a couple of steps
- Talk about readings and data integrations
- Work on final project idea in the second half of class, then share and get some feedback

Coding Exercise for Portable Information Structure Definition:

- Pull up discussion thread with definitions from last week, copy into a spreadsheet, one per row, then start coding the definitions for common themes and phrases that occur across definitions
- Make those themes into columns, mark which definitions include those things to see what are most commonly included
- Will then add those common themes into a template to come up with a working definition for the class
- From exercise, key words that class came up with were:
    - Interoperability
    - Standardized
    - Easy to understand
    - Transfer
    - Privacy
    - Human & machine readable
    - Self-descriptive
    - Security
    - Common formats
    - Transparency
    - User access & control
    - Reusability
- Condensing terms led us to this list:
    - Common formats & interoperability
    - Transparency & easy to understand & user access and control – each are a different aspect of transparency
    - Self -descriptive & easy to understand
    - Human and machine readable & easy to understand
    - Common formats & standardized
- For each of the pairs above, see which term we can drop to create a more precise definition. Narrowed list down to this:
    - Standardized formats
    - Human & machine readable
    - User access and control
    - Reusability
    - Transfer
    - Privacy
    - Security
- Insert the terms into a definition template:

Portable information structure

Is a _standardized format_ (type)

That enables _user access and control, transfer_ (enables what)

Across _different systems_ (contexts)

By using _standardized formats, reusability, human & machine readable_ (key properties)

While addressing _privacy, security_ (constraints)

So that _human and machine readability_ (outcome)

- Final definition draft:

Portable information structure is a standardized format that enables user access & control and transfer across different systems by emphasizing FAIR (findable, accessible, interoperable, reusable) while addressing privacy and security so that human and machine readability is possible

- Knowledge graphs: would be able to find synonyms of words to keep in clouds that could then be plugged into definitions

Discussion on readings:

Reading 1:

- Readings selected as inspirations or templates for final project – diversity of ideas and examples that project could be mapped to
- Examples of more structure and metadata being added to create more meaning
- Professor worked on a project to do fuel estimation using a camera that went across the ground
- Fuel estimation reading is a good resource for knowledge graphs – ultimately, knowledge graphs are great for integrating data – create a model of relationships, and then map data to those relationships
- Linked open data started by Tim Berners-Lee, thousands of concepts and relationships, gives standardized framework
- Search engines use schema/ontology to tag pages – schema.org

Reading 5:

- Chatbots before generative AI
- Importance of being user driven
- G3 is about thinking about what the user would want
- Before generative AI, it was difficult to have open ended conversations – had to have pre-framed questions that came from understanding the user – ground down to an information story that the app supports

Reading 3:

- Example of accessibility being the most important aspect
- API to allow for accessibility that other people can then build on – “data mash ups” by combining different APIs to make a new API

Reading 2:

- Several examples of why integrated data helps businesses and people, examples from different industries

G3 assignment:

Making an information story and structure:

- Data that is out there today is the result of some sort of process – process happens, data is stored in file
- Most useful data is that which has been integrated
- Fuels data and physics data took data source and then integrated more domain knowledge into the dataset – standardized format, but also more human readable by providing context and definitions
- When taking a dataset, what are the things in there that could be defined
- W3C standards, or DBpedia (sematic web database) – cross reference information and provide structured data
- Readings bring in more data that makes data more self-describing, links to other identifiers
- Think of data source or data set that you use regularly that is integrated or requires integration
    - Weather app providing temperature and the feels like temperature (takes wind, humidity, sun into account)

In class activity time:

- Can use ideas from prior week, or come up with new ideas for this assignment
- Goal is to get closer to final project idea or theme
- Add an information story, and how you would want to structure the information to increase portability
- What to add in the submission JSON – pick top idea, give idea a descriptive name, summarize what the idea is about, information story, possible structure
- What is an information story:
    - Example: As a student I need access to the building, need keycard to scan to get into the building to be able to go to class – student information needs to be in database, and access needs to be enabled
        - Stepping back, the information could have been to create the card reader – need to integrate information from student and faculty database, the class times and locations, which is then connected to the card reader – enables access to the assigned class, maybe has some limitations to only do 15 minutes before and 15 minutes after – actual system uses local look up
    - Information story is like a user story but emphasizing the information – what is the journey that happens
- Examples of projects shared in class:
    - Have a filtering mechanism for all the noise on the internet, to be able to just see the social media content that you want – create a taxonomy for the AI agent to work with and make decisions on your behalf of what content to see. Professor likes this idea and the integration of new technology.
    - Taking data for King Country Transit System (timetable, GIS data, routes) and putting it in a knowledge graph – could then do a node visualizer for relationships between stops, could also do a stress test by taking out nodes – for a user, could choose a certain stop and their commute. Alternatively, see what their alternative routes and stops could be if their stop is not accessible. Feedback from professor: think about a more refined user story, calendar integration would be interesting because it increases accessibility.
## Week 3, Session 2 Class Notes
### In Class Notes:

- We are back to a wintery clime, with rain across the greater Seattle area
- Project vs student group clarification– resolution: if student groups are made, prof can convert to project groups without too much issue
- [https://medium.datadriveninvestor.com/access-companies-sec-filings-using-python-760e6075d3adLinks to an external site.](https://medium.datadriveninvestor.com/access-companies-sec-filings-using-python-760e6075d3ad) is a paid article, the instructor will find an alternative

- Tending the garden of functioning links

- Web 3.0: Borge’s garden of ever-pruning paths

- Today, theme is machine:machine translation and working on individual assignment [I3 Build Lightweight Application](https://canvas.uw.edu/courses/1883881/assignments/11160559)
- Working and sharing session for I3 to discuss things we’ve run into building that
- Github/Collab notebook setup, discussion of what Github is like
- Monday, discussed info stories– reason/power of placing a user (and needs/goals) to guide structuring information

Final project theme: goal to visualize, analyze, predict, or automate _something_

Goals:

- Exposure to more technology
- Info system stack
- Converting data to useful form
- Similar angle to user story
- Visualize/understand something about the world, info if it allows visualization, is positive

Info can be in difficult to visualize structure

Importance of data warehouses in BI– vast, responsive, interactive visualization to allow targeted querying dynamic responses

BI systems get us to an information structure that allows for visual understanding and decision making– decision support

Info structure created from data warehouse

BI systems are created out of taking disparate systems, ETLing them, mapping them with metadata into a new series of structured representations (dimensional models, snowflake/star schemas) with facts and dimensions that drive views that answer questions

The view becomes the information structure for a given use case

When we talk about info structures being made portable, what we’re doing is building same infrastructure of BI architecture

Business question is what drives whole BI activity to build bespoke view of data to answer questions

We want to do the same thing with portable info structures, making them more useful as is

Some information structures (data.gov, Seattle city gov JSON structures), point of websites is to make data both open and usable– not an easy balance to strike

In the BI case, if we removed business question, the whole process has no focus/aim and it is hard to usefully make meaning of the assembled dimensions

Without focus/use/business question, we don’t know what views to construct

- Predicting: info structure supporting recommendation task using prediction

- Google Maps: search for gas station, coffee, gives recommendations sorted by some internal order– distance, time to get there, number of transfers

- List of options of type queried, facets to filter list generated
- GIS Data
- Operating hours, whether they accept credit cards, parking availability, food options, contact information

- All servicing one BI view for one use case to query disparate databases
- Structuring to give dynamic user activities

- Netflix: prediction of what will engage users– balance between personalized for user and trending/popular among genpop

- User Interest maps, viewing habits
- Movie catalogue
- “Something you’re going to want to watch”: algorithmic engagement prediction
- Your experience is tailored to drive engagement metric
- Automation combined with analysis, prediction

- Automating: 
- Analyzing: 

Structuring information for 

Two levels of machine work happening with prediction:

1. Machine:machine structuring to create dataset– based on distributed infosystems

2. Not just a set of data that exists, aggregating endpoints to serve application
3. Machine translation to single structure

4. Machine:human translation to make user operable, made to enable user comprehension

5. Extra analysis performed on results to drive usability

Ex:  {“idea”: “main”, “Summary”: “idea”} Is not that helpful for feeding to a second machine to generate recommendations, considerations of machine understanding, data type

What we’ve focused on so far is human comprehensibility and accessibility

**Now shifting to gearing towards building infostructures for machines**

Readings have examples of different application types to create visualization

### Example: Federal job search developer article discusses ways of finding jobs via USAJOBS API

What would be use case for pulling those API results: 

- Visualization: graph trends of job posting over time– historical data

- Insight about which industries/professions are worth looking into– what kind of jobs to apply to
- Historical, visualizing cyclical hiring trends/seasons

- Automation: 

- Repost top/relevant jobs
- Automatically applying to jobs

- Related: application preparation– this needs other data to be pulled in, cover letter context, templates, your own resume

- Company research– how big is the company, how many times has this job been posted, how often are they hiring

- Insight: 

- Job requirements, pull data to understand commonality of certs/skills/YoE

- Analysis: 
- Prediction/recommendation: 

- New jobs that match user selected criteria, digest of 10 recommended jobs that match my skills

Insight we’re trying to drive is both visualization and “these are the jobs you should apply to: top 5 of trending, top 5 to avoid”-- the insight derived from visualization is what’s valuable, the visualization is worthless without insight in mind

Insight in mind drives which fields to bring in

  
  

### Example: [https://www.storytellingwithdata.com/makeoversLinks to an external site.](https://www.storytellingwithdata.com/makeovers)

Tableau has examples of great visualization– if you have dataset available, tell a different insight or improve storytelling

Example: Kaggle [EDGAR APILinks to an external site.](https://www.kaggle.com/code/svendaj/extracting-data-from-sec-edgar-restful-apis) article

Example: Python [Web scraping tutorialLinks to an external site.](https://realpython.com/python-web-scraping-practical-introduction/)

10 mins to find info structure we can access and use for [I3](https://canvas.uw.edu/courses/1883881/assignments/11160559):

- Can be info structure for group project, but can be personal thing
- Want ready made structure to brainstorm uses/insights to derive from that

Github: 

Call it whatever we want

Best to be public to allow reader/grader access

Recommended: create folders to get structure started now

All doable via web UI, don’t have to worry about git process

Markdown is simple for this purpose: # is a header, ## is a subheading

  
  

Capture structure we’re thinking about using via markdown

Capture insight we’re deriving via 

Resources to think about how to approach building I3 technology stack: 

- Assignment is building a light-weight application– usage of these words is loose

- Application could be Python/Jupyter notebook, webpage of HTML, visualization in viz tool (Excel, PGAdmin4)
- Goal is to be visualizing, predicting, automating, analyzing _something_ 
- Can be new information, can be from previous
- Create ReadMe file to describe how to use information– allow peers/prof to test
- Don’t have to use Python, generative AI allows us to branch out into a wide variety– decide pain tolerance for frustration
- Go through process of using existing structure to gain insight, exposure to applications using infostructures
- ReadMe tells reader why project is useful, what can be done with it– what the driving business question is
- Colab notebook is a good place to start

- Text mining example: [imt576_textmining.ipynbLinks to an external site.](https://colab.research.google.com/drive/1gl_ccaIPlznIiRtZEQUwmmdvoCWwQOQU?usp=sharing)

Colab general example:

- Install libraries required
- Set up API headers to backend
- Issue API request to get specific info from website
- Use API info to get info structure about assets, hardcoded CIK number
- Transform responses into a flat structure
- Use plotting tool to plot insight
- Outputs graph (in this example)

Edgar Earnings Transcripts: 

- Earning transcript is text, using webscraping

- Go to “Seeking Alpha” earnings transcripts webpage where people talk with leadership

- Use print option, select all, copy text into github as a new file as earningstranscript.txt

- Can then text mine transcript, commonality of words, natural language processing

General class plan:

- Python– local
- Python– Colab
- Python– Jupyter, include lines about required libraries/dependencies

- Either download VSCode, Jupyter

- Notebook in Git allowing people to select

- Can take notebook and make Python executable locally

- Javascript docker container
- Flask server

### Responses for what we were surprised by/see as challenges as we start to look at data structures:

- Challenges: 

- Scoping to be done on project, determine what data to curate from dataset to be written to portable format– challenges of open-endedness

- Suggestion: think of very specific use case, solve that, then zoom out

- Reddit API hard to obtain, workarounds to avoid

- Describe in markdown the challenges you encounter, sometimes you realize there’s a simpler way– info doesn’t have to come from API

- Analyzing item name to match with USDA generic name
- Data quality issues– Bluesky API, processing required
- Too large of datasets or specific question– either change question to have dataset work, or use different dataset to serve purposes
- Have to enrich dataset

- Don’t need to do integration if unnecessary, can just develop insight/analysis from one source

## Week 4, Session 1 Class notes
## **General Architecture**

**Building Architecture Examples:**

- Visiting sacramento
    - Lots of flat buildings
- Crossroad's mall food court
    - People coming in and out
- The Quad Gargoyles
    - Presence of academia and history
- City Campuses
    - Efficient spaces, small rooms

**As an architect:**

- Inhabit that space and where/what your users are using it for
- As an information architect
    - Take in user requirements, and understand the general structures and objects themselves

**Difficulties of architecture:**

- Typically designed for a feature or a technology, not for users
- User Stories
    - Boundary objects
        - To allow people to form collective understanding or shared understanding
        - Sense-making
        - Apply this into projects, what are the users wanting to do with your project? 
    - Takes us away from how to do something, makes goals of the system readily available
    - In business contexts and expertise, user story focus differs, recognize what others may prioritize as well

## **Digital Information Product Development Article (Keller & Lima)**

- Case study on a new product development (NPD) process from ABC Online-Marketing
- Stages and processes in NPD process
    - **Meyer & Zach's Theoretical Framework (Interactive-iterative)**
        - Product Conceptualization
        - Acquisition
        - Refinement
        - Storage Retrieval
        - Distribution
        - Presentation
        - Market Feedback
    - **Case Study (ABC Online-Marketing)** 
        - Idea generation
            - Market research, what their competitors are doing, internet research, customer conversations
            - Networking
            - Ideas inside the firm, more common as informal conversations to ensure creativity
            - Typically, there is a high degree of informality and curiosity from other perspectives to understand what user needs are.
                - You need to validate it, talk to other people, talk to customers, etc...
            - Continuous process, not something that just comes and goes.
        - Idea validation
        - Product creation
        - Product launch

Where does the information of the user story come in?

- Conceptualization & Market Feedback, validated product launch

## **G4 Assignment slides**

Four main components, slides 1-3

- Information user story V.S existing procesess/systems
- Wireframes
- Main concepts
- Architecture system

Think of what the user is trying to do, not what is necessarily in the data.

- Is there enough information and data for a story?
- Hard to make a product if we don't have enough data to assess?
- Re-iterative process, do customers need this? Can the business sustain this?
    - Without considering the four components, you end up with products that won't be utilized. 

Call back to Case Study process 

- Idea generation
    - Think of people who YOU can talk to/discuss your project
- Idea validation
    - Validate by getting more perspectives
- Product creation
- Product launch

G4 Assignment feedback session, general runthrough

## Week 4, Session 2 Class Notes
### **1. Where Does Data Come From?**

#### **Example: Airplane Engine Temperature**

- A **temperature sensor** captures analog temperature in the engine
- A computer converts the analog signal to a **digital format** (e.g., 180°F)
- Data updates **once a second** and is stored in hardware

#### **File Format Attributes**

- **Metadata**: CSV, JSON
- **Data types**: int, str
- **Compact formats** → useful for high volume of data
- **Binary fields**: stored bit by bit (bit: sign)(bit: type)

### **2. File Types & Formats**

#### **Brainstorm: As Many Types as Possible**

**Text-readable (human-readable):** Text, JSON, XML, HTML, Markdown, CSV, RSS, YAML, DOCX, PPTX, LaTeX, GML, RTF, PLS, RDF

**Other / Binary formats:** JPG, ZIP, TAR, Spreadsheet, PDF, HTTP, JAR, RAR, SAV, MKW, MP3, WAV, GIF, PNG, MP4, ICO, EXE, INDD, MOBI, PY, IPYNB, AI

#### **Why Are There So Many Formats?**

- **Proprietary / Lock-in ecosystem** — vendors create formats to keep users within their tools
- Even though many formats are text-readable, different formats exist because of:

1. **Structure / Predictability** — e.g., if we see JSON, we can predict the data layout
2. **Accessibility** — different tools and users need different formats
3. **Portability** — some formats transfer more easily across systems
4. **Historical reasons** — some formats exist because they came first (better alternatives found later)

→ We get benefits like **structure, accessibility, and portability** through **conversions and compression**.

### **3. Technologies for Accessing & Manipulating Data**

#### **Getting Data from a Data Center**

- **API** — HTTP server that accepts requests
- **Curl** — command-line tool for making HTTP requests
- **SCP, SFTP → SSH** — secure file transfer protocols
- **CLI** (Command-Line Interface) — interact with data via terminal
- **SDK** — Software Development Kit for programmatic access

### **4. Lab / Assignment: Work on I4**

- Experiment with different **data access methods**
- Define: **What is the use case and file you're using?** Tell the story.
- Professor suggests using **Google** **Collab**:

- Write down the code
- Add documentation

- Tools & concepts to explore:

- **Website / URL** — fetching data from the web
- **Beautiful Soup** — Python library for web scraping / parsing HTML
- **Call API using Collab agent**

## Week 5, Session 1 Class Notes
Took FAIR Quiz and discussed answers

Broke up into 4 groups, each given 10 minutes to understand and prepare to teach one area of FAIR.

Findable:

- Findable refers to reference points to data and metadata for indexing and references
- URIs, uniform resource identifiers, can be HTTP like likes, or DOI reference points.
- Referenceable by humans and computational quizzes.
- Reference to meta data should also be referenceable and searchable.
- DOI are often found on journal articles, can be found.
- Digital object identifier
- Assigned by DOI registration agency, like publication office of European Agency, government agencies
- [orgLinks to an external site.](http://doi.org/), foundation manages registration
- To be a registering agency must agree to some principles, including around IP
- How to get a URI
- A URL would work, but not all URIs are URL
- Need a hosting site
- URI’s have an allowed character set to make them readable,
- Wikipedia has a nice description of structure: scheme, authority, host, domain, port, path… /forums/questions…

Accessible

- Need to be able to find the metadata, usually through HTTP or FTP as a common protocol to find metadata, and same for data
- Protocol for authorization should be open and standard, doesn’t mean everyone should have access to
- Shouldn’t data be free? Some data is sensitive, should be accessible but not to everyone. What about non-public data?
- Anecdote about corporate research with internal, classified, and public data, allows the internal knowledge management and librarians to organize and give access. However, when the culture to manage doesn’t include FAIR principles, the public white papers and information that could have been given DOIs or persistent identifiers may not be present and that meta data (and data) gets lost.

Interoperable

- For data to be integrated with other data, needs properties to be under stable with syntax to be readable by humans
- Needs global approved codes
- Scientific links need to be described
- Data integration needs to be documented
- Data sets need to have recognized vocabularies
- Metadata should also follow FAIR

Reusable

- Mostly about the metadata associated with data set
- Metadata should provide as much as information as possible
- If you are creating the metadata, you shouldn’t assume anything about the user but provide as much detail as you can
- Be clear about the licenses of the data and if you used any data that had licenses
- Some industries may have standards that you should follow
- Tools exist to help you track licenses
- If you transform a dataset, tell how you did that
- Minimum information standard, in R3, a community standard where if you work with specific data, you should follow their practices
- Make sure that the data is useful for machines and humans

What should our portable info structures include?

- Metadata,
- check out what already exists,
- licensing

What from FAIR doesn’t apply to portable information structures?

- Metadata indexed may beyond scope of the class.
- Minimum information standard, as a community standard

How to apply reusable, in an agentic way?

Read one example from the paper about FAIR, UniProt example, that demonstrates what G5 is all about.

Spent 10 minutes looking at other examples to find similar places group projects are implementing FAIR as well as potential additional ones.

Observation discussion from that exercise:

- Starting from an existing information structure, like from Seattle public transportation, that has already put effort into portability and FAIR principles makes it easier to extend and continue with FAIR adherence
- Having multiple formats in existing structure, like JSON and html, provides options for increasing portability and idea that the new structure should include those formats
- A genAI agent that creates knowledge base facts should also adhere to FAIR principles as it’s creating information it will use later

Ended on discussion point that perhaps, in FAIR, where the common use concept is that the data and metadata should be useable by humans and machines needs to include Agentic AI. Point was made that HTML is for machines to render effectively in a browser, while Markdown is a simpler format for rendering documents, but is much smaller. So an Agentic system may prefer the more compact MD but could lose information that an HTML system had. Also, Agentic systems were trained and should understand really well HTML, but perhaps MD is good. Interesting things to think about with Agentic AI now part of information systems.
