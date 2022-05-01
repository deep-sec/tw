# HashiCorp Engineering Writing Style

Whether it is a blog post or technical documentation,
HashiCorp has a particular writing style we do our best to adhere to.

## Why?

A consistent writing style and voice makes the HashiCorp brand
strong and vibrant. There are a few reasons for our writing
style choices. In particular, we want to optimize for:

- **Non-native speakers** - Translations are not literal in different countries or regions.

- **2am, half awake operators** - Flowery sentences are not helpful when trying to
  get a system back online.

- **Time efficiency** - When we write in the same style, we can
  spend more time focusing on the content.

- **Product transitions** - Users familiar with Consul documentation can adopt Vault without learning a new language. 

## Guiding principles

Experience and user feedback guide the majority of our principles. As a
high-level set of rules, we follow [Orwell's 6 rules](http://www.orwell.ru/library/essays/politics/english/e_polit):

- Never use a metaphor, simile, or other figure of speech you see in print.

- Never use a long word where a short one will do.

- If it is possible to cut a word out, always cut it out.

- Never use the passive where you can use the active.

- Never use a foreign phrase, a scientific word, or a jargon word if you can think of an equal one in common English.

- Break any of these rules sooner than say anything outright barbarous.

## Sentence structure

We have three main rules for sentence structure listed below. 

### Active voice

To convey causality, always use active voice. For example:

- This file configure ...
- Terraform deploys ...
- The proxy sends ...

### Present tense

To convey the timing, always use present tense. For example:

- Now configure the server.
- Set the variable ...
- Add the parameter ...

### Directive language

To convey action, use directive language. For example:

- Open a browser. 
- Download the binary.
- Destroy the infrastructure. 


### Complete example

```text
Good:
To install Terraform:
1. Find the correct package for your system.
2. Download it as a zip archive.

Bad:
You can install Terraform by finding the binary and downloading it. You will need the appropriate package for your system.
```

## Word choice

The following are recommendations that will help you with word choice. 

- Use "you" for the user.
- Use "we" for HashiCorp recommendations.
- Avoid 'ableist' language.
- Never use a metaphor, simile, jargon, or other figure of speech.
- Use short words.
- Cut unnecessary words.

Below are a few word-choice examples. 

### Grammatical person: "You" for the user

Write docs in the second person and address the reader as "you".

```text
Good: Terraform Cloud's API lets you create workspaces without a VCS connection.

Bad: Terraform Cloud's API allows one to create workspaces without a VCS connection.
```

### Active voice: "We" for HashiCorp

Active voice _enforces attribution._ In
our documentation, the opinions and advice on offer belong to **us, here at
HashiCorp.** Our language should never try to hedge or evade responsibility for
the guidance we're providing. If HashiCorp is making a recommendation, say "we".

```text
Good:
We recommend configuring VCS access when first setting up an organization.

Bad:
It is recommended to configure VCS access when first setting up an organization.
```

In cases where the actor of a sentence is a tool or system, rather than a person
or company, you should still use active voice. It's easier to
understand and sometimes distinguishes between automated and operator actions.

```text
Good:
Next, Kubernetes will register the service.

Bad:
Next, the service will be registered.
```

### Inclusive Language

### Pronouns

To cut down on the number of pronouns in your writing, replace the user with the grammatical person "you". If you do find yourself using pronouns,
make sure they are necessary, and if so, use the gender neutral "they/them".

|Good|Bad|
-|-
|Once you give the developer the token they can...|Once you give the developer the token she can...|

### Over Simplification

Our products are rich and complex. Avoid using words that allude to processes being easy. Doing so can alienate users who are having a hard time or are encountering bugs.

Avoid saying:
- easy, easily, simply
- just (as in "just run this command")
- obviously
