# Challenge Rules

In this file it is outlined the rules and operation for the Challenge. Be sure to give this a thorough read to make sure your submission gets a nice score and you don't miss the submissions deadlines!

## Steps and Deadlines
The challenge is divided into 3 steps, with their deadlines yet to be defined:

1. CURRENT -> **Registration** - Participants register their group.
2. **Development** - Participants develop their Addons and submit their challenge solution.
3. **Evaluation** - The judges will give their Score to the submissions, and a community poll will be up.
4. **Presentation** - The poll is closed, the challenge results will be revealed, and the prizes distributed.

## What You'll Create
Here are some basic information about what your Addon will need to handle. A couple of them come from details of Meta-System and are explained thoroughly in the documentation. Next is a quick summary of what matters most for this challenge.

> You can join the [Meta-System Discord](https://discord.gg/ndGsnbTW7V) or Send a DM to Zelcion on [X](https://twitter.com/ZelcionV) or Discord for clarifying any question you may have.

#### Informations
- 👉 **Schemas** can have any format, including being deep. The schemas used to evaluate the Addon won't be revealed until the challenge submission period ends. [See here about the Schemas](https://mapikit.github.io/meta-system-docs/docs/api-docs/configuring/schema-config).
- 👉 **Schema Functions** have only a single parameter which is an object. The addon can specify what the format of this object is. Their output must also be an object. [See here about Schema Functions](https://mapikit.github.io/meta-system-docs/docs/guides/broker#entity-schema-functions---brokerschemafunctions).
- 👉 **Schemas** can change format between initializations.
- 👉 **The Addon** may not validate its Schema Functions input. This is done in Meta-System through its configurations. 
#### Requirements
- ❗**The Addon** must be able to deal with N amount of schemas.
- ❗**The Addon** must be able to handle a Schema that changes formats between initializations without breaking the table. It is acceptable for data in changed keys to be deleted.
- ❗**The Addon** must have at least one Schema Function for each of:
  - **C**reating an entity
  - **R**etrieving entities with a query
  - **U**pdating entities with a query
  - **D**eleting entities with a query