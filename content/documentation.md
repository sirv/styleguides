# Documentation

### References:
[Sirv's documentation design guidelines](/design/documentation.html)

Sirv technical content appears in the [Help Center](http://sirv.com/help/) and throughout the app.

## Basics

Our overriding goal is for people to people to tell us "I love your documentation!". Now that's not something you hear very often! But it is possible, by making it expertly written, beautifully designed/illustrated and easy to navigate. Take a read of the [advice and examples for great documentation by Zapier](https://zapier.com/engineering/great-documentation-examples/).

Someone reading technical content is usually looking to answer a specific question. That question might be broad or narrowly-focused. Either way, our goal is to provide answers without distraction ASAP, leaving a positive impression on them.

For each project, consider your audience’s background, goal and current mood. Ask these questions:

- Is the reader a prospective user, a new user, or an experienced user?
- What is the goal of the reader? To complete a task? To research a topic?
- Is the reader in the middle of a task? Are they in a hurry? Could they be frustrated?

We should avoid overloading a reader with unnecessary information, choice, or complex ideas or phrases, when we don’t have to. This is particularly critical when a user may be new and/or frustrated. When relevant, prime the reader with a brief outline of an article’s focus in an introductory paragraph or section and stick to the topic at hand. Keep sentences, paragraphs and procedural steps focused and concise.

## Types of technical content

Technical content articles vary in target audience, goal and tone. Sirv technical content is built from these templates, which serve different purposes and readers.

| **Article Template**   | **User Type**          | **Goal**                                                                                                                                          |
| ---------------------- | ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------- |
| Getting Started        | prospective, new       | **Overview.** Include brief outline of topic, uses, benefits and related topics. Use links to best practices, cheat sheets and feature overviews. |
| HTTP API documentation | all                    | **Reference.** Summarise each option with an example ([imgix succinct example](https://docs.imgix.com/apis/url/mask)).                            |
| S3 API documentation   | all                    | **Reference.** Provide guidance and sample scripts for connecting to Sirv S3 with common scripting languages.                                     |
| Guides                 | new, intermediate      | **Guidance.** Detailed Briefly describe a task, provide a roadmap and pre-requisites and clear step-by-step instructions.                         |
| Tutorials              | new, intermediate      | **Guidance.** For common use cases, briefly describe a task, provide a roadmap and pre-requisites and clear step-by-step instructions.            |
| Best Practices         | all                    | **Context.** Make connections between Sirv and asset management / image hosting / web development / ecommerce as a whole.                         |
| Cheat Sheet            | intermediate, advanced | **Reference.** Quick reference to common scenarios.                                                                                               |
| Blog articles          | prospective, new       | **Marketing.** Interesting articles about Sirv features, benefits, customers, uses and new updates.                                               |

## Guidelines

### Drafting technical content

Before you begin writing a new article, speak with an expert at Sirv (like an engineer, designer or technical support advisor) to get as much information as possible. You may only use a small portion of what you learn, but it helps to have more information than you need to decide where to focus your article.

Consider how many articles are needed and what article types will best describe a new feature or tasks to the user.

Outline your article, then write a draft. Stay in touch with your subject matter expert and revise as needed for accuracy, consistency and length.

When you’re happy with a draft, pass it to another technical writer for peer review. For new content or highly complex content, send your final draft to your subject matter expert for approval.

### Writing technical content

When writing technical content, follow the style points outlined in the [Voice and tone](https://github.com/sirv/styleguides/tree/main/content/voice-and-tone.html) and [Grammar and mechanics](https://github.com/sirv/styleguides/tree/main/content/grammar.html) sections. Here are some more general pointers, too.

#### Stay relevant to the title

When a user clicks the title of an article, they expect to find the answer they want. Don’t stray too far from the title or topic at hand. Use links to make related content available. If you find you’re getting too far from the intended topic, then you may need to create a separate but related article.

#### Keep headlines and paragraphs short and scannable

Focused users often scan an article for the part that will answer their particular question. Be sure headlines are short, descriptive and parallel, to facilitate scanning.

#### Use second-person and describe actions to a user

Technical content talks to users when support agents can’t.

#### Strive for simplicity and clarity

Be as clear as possible. Use simple words and phrases, avoid gerunds and hard-to-translate idioms or words, focus on the specific task, limit the number of sentences per paragraph.

#### Provide context through embedded screenshots, GIFs, videos

Screenshots, GIFs and vidoes are often ideal to help orient new users. Crop screenshots tightly around the action to focus attention.

### Editing technical content

We edit technical content based on three goals:

**Digestibility**

- Cut or tighten redundancies, gerunds, adverbs and passive constructions.
- Use the simplest word.
- Limit paragraphs to three sentences.

**Consistency**

- Use the labels and terminology used in the Sirv web app.
- Use specific, active verbs for certain tasks.
- Choose basic words and phrases to facilitate consistency across translated content.

**Helpfulness**

- Stay conversational, using contractions when appropriate.
- Avoid qualifiers that muddy meaning.
- Express understanding when appropriate.
- Craft clear transitions from section to section to orient the reader.

### Formatting technical content

Technical content uses organization, capitalization and other formatting to help convey meaning.

#### Capitalization

Capitalize proper names of Sirv products, features, pages, tools and team names when directly mentioned. In step-by-step instructions, capitalize and italicize navigation and button labels as they appear in the app.

- Sirv, Sirv Spin, Sirv Zoom
- Settings page, Profiles folder
- Support Team, Development Team
- Navigate to the *Settings* page.
- Click *Save & Close*.

#### Headings

Group article content with H2s and H3s. Use H2s to organize content by higher-level topics or goals and use H3s within each section to separate supporting information or tasks.