# RFCs

## What is an RFC?

An RFC describes a change to Alchemy, for example a new feature or UI change. Any substantial change should go through the RFC process. Each RFC is proposed as a pull request to the `alchemy-rfcs` repository, is reviewed, and ultimately is either approved or rejected.

## RFC process

### 1. Create a new RFC

RFCs are numbered, starting at `0001`. To create a new RFC, create a new branch of the `alchemy-rfcs` repository. Check the existing RFCs to identify the next number to use. Then, copy the [RFC template](https://github.com/dorgtech/alchemy-rfcs/blob/master/rfcs/0000-template.md) to a new file in the `rfcs/` directory. For example:  

```sh
cp rfcs/0000-template.md rfcs/0015-membership-actions.md
```

Write the RFC, commit it to the branch and open a [pull request](https://github.com/dorgtech/alchemy-rfcs/pulls) in the `rfcs` repository.

In addition to the RFC itself, the pull request must include the following changes:  
- a link to the RFC on the [Approved RFCs](./approved.md) page

### 2. RFC review

After an RFC has been submitted through a pull request, it is being reviewed. At the time of writing, every RFC needs to be approved by  
- at least one dOrg team members
- at least one DAOstack team members

### 3. RFC approval

Once an RFC is approved, the RFC meta data (see the [template](https://github.com/graphprotocol/rfcs/blob/master/rfcs/0000-template.md)) is updated and the pull request is merged.
