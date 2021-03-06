![in progress](https://img.shields.io/badge/status-in%20progress-yellow)


# Phase 4: Review data model and incorporate comments
![Process_Phase 4](img/methodology_phase4.PNG)

**Quick links:**
- [`Step 13`. Review draft data model](phase4.md#step-13-review-draft-data-model)
- [`Step 14`. Propose enhancements](phase4.md#step-14-proposition-enhancements)
- [`Step 15`. Propose additional attributes](phase4.md#step-15-propose-additional-attributes)
- [`Step 16`. Perform semantic mapping of attributes](phase4.md#step-16-perform-semantic-mapping-of-attributes)
- [`Step 17`. Harmonise, entities, attributes and descriptions across the data model](phase4.md#step-17-harmonise-entities-attributes-and-descriptions-across-the-data-model)
- [`Step 18`. Update draft data model](phase4.md#step-18-update-draft-data-model)

**Navigate to the different phases**\
[:arrow_left: Previous phase](phase3.md) **|**
[Next phase :arrow_right:](phase5.md)

## `Step 13` . Review draft data model

**Key activities**

> * The [<b>Working Group members</b>](../stakeholders#working-group) directly review the proposed model and/or contact domain experts for reviewing it. 
> * The [<b>editors</b>](../stakeholders#editors) moderate and classify the issues (e.g. tag major issues which should be commented in priority by the reviewers).

<details>
  <summary><b>Description</b></summary>
  
  Each published draft of the Data Model is reviewed by the Working Group members and domain experts when relevant. 
  
  Beforehand, the Working Group members and the editors agree on a tool to collaborate and capture the feedback. The reviewers can then create issues using the designated tool. When comments are captured outside of the collaborative tool, the editors make an issue out of them in the issue tracker (for each comment). 

  The editors respond within an agreed timeframe to each issue, informing the reviewer that they have noticed and will process the issue. The editors consolidate solutions to the issue and seek for additional contribution from the reviewers (i.e. remainder of the Working Group members) when needed in collaboration with the moderator and rapporteur.
  
  The issues can be in many different forms. For instance, a issue can deal with a modification to an existing entity or attribute, the addition or removal of an entity and/or attribute. For further details about these the types of issues, please check; 
  
  * [`Step 14`. Proposition enhancements](phase4.md#step-14-proposition-enhancements)
  * [`Step 15`. Propose additional attributes](phase4.md#step-15-propose-additional-attributes) 
  
  In addition to that, an issue can be qualified as `major issue` in the case it requires specific attention from the Working Group and the reviewers for commenting the issue and the potential resolutions. Further categorization (i.e. [labels](https://github.com/SEMICeu/SDG-sandbox/labels)) is proposed when registering an issue.  

  The moderators make sure that the agreement process is transparent and acknowledged by all reviewers. Concerning *how consensus will be reached* you can find more information [here](../process_and_method/review_cycles_and_consensus).

</details>
<details>
  <summary><b>Rules and guidelines</b></summary>

* Reviewers are encouraged to directly create issues on the collaborative tool.
* Reviewers are encouraged to propose a solution in case they raise an issue. 
* Reviewers are encouraged to use labelling and tagging for increasing searchability and responsiveness of contributors.
* Reviewers should consider how to present and discuss issues (e.g. technical versus business aspects).
* Reviewers are encouraged to provided context to their issues (e.g. data models used).
* Reviewers are encouraged to structure their issues and especially their denomination to increase comprehension. For instance: 

```diff
Name of the data model or sub-part (e.g. relevant entity) and a short statement of the issue

+ VehicleRegistrationCertificate evidence should contain registration status
```
</details>
<details>
  <summary><b>Tool(s)</b></summary>
  
  We propose to use GitHub as the preferred tool for reviewing the data models. Github is a collaborative tool with built-in versioning control as well as other features that make it easy to propose suggestions and raise issues. ([Here](https://docs.github.com/en/github/managing-your-work-on-github/creating-an-issue) you can find the documentation on how to create issues on GitHub.) Nevertheless, other tools such as Jira or Confluence, can also be chosen. There are some important aspects to consider when choosing a tool, on which we elaborate next.
   
  <details>
  <summary>Key aspects to consider w.r.t. the chosen tool</summary>
  
  *	**Proprietary vs open access and licensing:** 
  ```diff
  Are there licences or other requirements for accessing the tool?
  
  + GitHub: For contributing to a public repository, GitHub asks to create an account with a valid email address.
  
  What are the licensing conditions?
  
  + GitHub: For public repositories, the administrator can decide which licence applies. GitHub provides guidelines for licensing public repositories. As the content of public repositories is publicly available, the licences proposed are open source.
  
  What are the limits of the free version?
  
  + Github: Each account created can use 1 GB of storage and 1 GB of monthly bandwidth for free. 
  ```
  *	**Archiving and persistence:** 
  ```diff
  Who is owning and maintaining the tool? 
  
  + GitHub: GitHub, Inc. owned by Microsoft is the organisation owning GitHub.
  
  Has the owner engaged to store the content for a certain period? 
  
  + Github: GitHub intends to keep public repositories available except if specific conditions are met (such as violation of Terms of Service).
  ```
  *	**User-friendliness and adoption**
  ```diff
  What is the current level of adoption of the tool?
  
  + GitHub: Most of the Working Group members are familiar with GitHub.
  
  How easily can someone learn the basics?
  
  + GitHub: Accessing and creating issues in GitHub is straightforward and well-documented. Additional features can be learnt along the way.
  ```
  *	**Security**
  ```diff
  Is the content restricted?
  
  + GitHub: There are no access restrictions for public repositories. 
  ```
</details>

</details>
<details>
  <summary><b>Example(s)</b></summary>
  
  The following example describes the `review of a draft data model` followed by the creation of an issue and its processing by the editors and Working Group members. The process is the following:
  
  1. The editors publish on GitHub the diagram and tables describing the [Vehicle registration certificate](https://github.com/SEMICeu/SDG-sandbox/tree/master/evidences/vehicle_registration_certificate/data_model).
  2. While reviewing the model, a semantic expert or a domain expert will try to answer the following questions:
  ```
     * Are the elements and their relationships correctly used and labeled?
     * Do you agree with the definition of the elements?
     * Are all elements necessary for this evidence described in the model?
     * Are there conflicts between the elements of the model and the elements used in your country?
     * Is the element mandatory or optional in your country (cardinality)?
     * Do you have specific codes or expected types (e.g. format of date, address etc.) for attributes?
  ```
  3. The reviewers document their issues on GitHub. For instance, concerning the [Vehicle registration certificate](https://github.com/SEMICeu/SDG-sandbox/tree/master/evidences/vehicle_registration_certificate/data_model), the following issue was created [#45](https://github.com/SEMICeu/SDG-sandbox/issues/45).

  ```
  You may notice that the issue describes in practice several comments related to the vehicle registration certificate as well as an image of the data model used within the country. 
  ```
 
  To simplify the contribution of other reviewers to this issue, the editors will analyse the proposition, categorise it with labels, verify whether the issue should be restructured and describe the pros and cons of the issue documented. 
  
  ```
  In our example, each bullet point from the general comment should represent a separate issue. 
  However, the editors should avoid as much as possible to complexify the structure of GitHub issues by creating complex hierarchies between the issues.
  For instance, the visual data model proposed by the issue owner does not need to be separated from the initial issue #45 since it represents a direct source of information which may be relevant for more than one issue. 
```
  4. The editors or the moderators answer, usually within one working day, to the initial issue created by ackowledging the issue or directly giving an initial answer.
  5. The editors give more details about the pros and cons of (the various resolutions for) the issue(s) raised to trigger the discussions and comments from other Working Group members. 
  6. The discussion continues as reviewers comment on the issue.
  7. When no agreement has been reached, the editors prepare the discussions and alternatives to be tackled during the next webinar following the public review period.

</details>

## `Step 14` . Propose enhancements

**Key activities**
> * [<b>Working Group members</b>](../stakeholders#working-group) propose enhancements after [reviewing the data model](phase4.md#-step-13--review-draft-data-model).
> * The [<b>editors</b>](../stakeholders#editors) consolidate the propositions and explain the pros and cons of the different propositions to the Working Group members. If needed, the editors seek for additional contribution from the reviewers in collaboration with the [<b>moderator</b>](../stakeholders#moderator) and [<b>rapporteur</b>](../stakeholders#rapporteur).

<details>
  <summary><b>Description</b></summary>
  
Working Group members create semantic issues which deal with `enhancements` to the draft data models published. Enhancements can take the form of new features or requests regarding the proposed draft data models. It can be adjustements to the definitions, relationships, datatypes, cardinalities, etc.

As outlined in [Step 13. Review draft data model](phase4.md#step-13-review-draft-data-model), the editors invite opinions and feedback to the issues and moderate the ensuing discussion.  
  
After consideration of the propositions, the editors record the resolutions and send a response to the reviewers. To a semantic issue, the response usually includes a summary of the context of the proposition, the resolution agreed by the Working Group and the justification for the resolution, particularly in case the proposition is rejected.

</details>

<details>
  <summary><b>Rules and Guidelines</b></summary>
  
  * The Working Group must resolve each proposition in one of three ways:
  
    * `Accepted`: This usually means that changes will be made to the data model that will be reflected in the next release.
    *	`Rejected`: No changes will be made to the draft data model.
    * `Partially accepted`: Part of the change is accepted, but other parts are rejected.
  
</details>

<details>
  <summary><b>Tool(s)</b></summary>
    <i>There are no specific tools for this step. Similar to the previous step, we propose to use the Github issue feature (or pull request feature for the more advanced users) to propose enhancements.</i>
</details>

<details>
  <summary><b>Example(s)</b></summary>
 
 ```
  TBD
  ```
</details>



## `Step 15` . Propose additional attributes

**Key activities**
> * [<b>Working Group members</b>](../stakeholders#working-group) propose additional attributes after [reviewing the data model](phase4.md#-step-13--review-draft-data-model).
> * The [<b>editors</b>](../stakeholders#editors) consolidate the propositions and explain the pros and cons of the different propositions to the Working Group members. If needed, the editors seek for additional contribution from the reviewers in collaboration with the [<b>moderator</b>](../stakeholders#moderator) and [<b>rapporteur</b>](../stakeholders#rapporteur).

<details>
  <summary><b>Description</b></summary>

Working Group members create issues which deal with `attributes (and entities)` that could or should be included to the draft data models published. It might be that in certain cases Working Group members request the deletion of an attribute and/or entity.

As outlined in [Step 13. Review draft data model](phase4.md#step-13-review-draft-data-model), the editors invite opinions and feedback to the issue and moderate the ensuing discussion.  
  
After consideration of the proposition, the editors record the resolution and send a response to the reviewers. The response usually includes the resolution agreed by the Working Group and the justification for the resolution, particularly in case the proposed attribute(s) is (are) rejected. 

</details>

<details>
  <summary><b>Rules and Guidelines</b></summary>
  
  The Working Group must resolve each proposition in one of three ways:
  
  * `Accepted`: This usually means that changes will be made that will be reflected in the next draft data model.
  *	`Rejected`: No changes will be made to the draft data model.
  *	`Partially accepted`: Part of the change is accepted, but other parts are rejected.
  
</details>

<details>
  <summary><b>Tool(s)</b></summary>
    <i>There are no specific tools for this step. Similar to the previous step, we propose to use the Github issue feature (or pull request feature for the more advanced users) to propose additional attributes/entities.</i>
</details>

<details>
  <summary><b>Example(s)</b></summary>

  For instance, issue [#26](https://github.com/SEMICeu/SDG-sandbox/issues/26) suggested to add the CO2 emission per KM as well as the environmental class attributes to the [vehicle class](https://github.com/SEMICeu/SDG-sandbox/blob/master/evidences/vehicle_registration_certificate/data_model/vehicle_registration_certificate_diagram_v0.09.pdf). 

</details>

## `Step 16` . Perform semantic mapping of attributes

**Key activities**
> * Upon receiving additional attributes from the [<b>Working Group members</b>](../stakeholders#working-group), the [<b>editors</b>](../stakeholders#editors) perform a semantic clustering of attributes. Afterward, editors will map the ‘semantic clusters’ to existing attributes, if any. Should there not be an attribute to map a ‘semantic cluster’ to, the editors will propose a new attribute (or entity). 
> * The [<b>Working Group members</b>](../stakeholders#working-group) discuss the ‘semantic clusters’ - and potentially the new attribute(s) - and work towards consensus. 

<details>
  <summary><b>Description</b></summary>
  Wherever attributes do not convey exactly the same information, ‘semantic clusters’ of similar attributes should be constructed to find a common, higher-level, and more general attribute to which the more specific attributes can be mapped. 
  
</details>

<details>
  <summary><b>Rules and Guidelines</b></summary>
  
  * The relationships among different attributes (or entities) can be given a value according to the [SKOS (Simple Knowledge Organization System_Mapping system](https://www.w3.org/TR/skos-reference/#mapping). The different values of which are
    * exact match
    * close match
    * related match
    * broader match
    * narrower match
    * (no match, i.e. absence of match)
</details>

<details>
  <summary><b>Tool(s)</b></summary>
  
  * This step can be performed using a spreadsheet tool, such as Microsoft Excel, in which related attributes are juxtapositioned in two columns and given a semantic mapping value in a third column.
</details>

<details>
  <summary><b>Example(s)</b></summary>
  
 ```
  speed hasCloseMatch velocity
  ```
</details>

## ` Step 17` . Harmonise entities, attributes and descriptions across the data model

**Key activities**
> The [<b>editors</b>](../stakeholders#editors) harmonise the entities, attributes and descriptions across the data model.

<details>
  <summary><b>Description</b></summary>
  The editors consider all the entities, attributes and descriptions across the data model and check their consistency. Editors may propose changes to the attributes, for example to harmonise the names and definitions across entities or solve inconsistencies.
</details>

<details>
  <summary><b>Rules and Guidelines</b></summary>
</details>

<details>
  <summary><b>Example(s)</b></summary>

```
  TBD
  ```
</details>

## `Step 18` . Update draft data model

**Key activities**
> The [<b>editors</b>](../stakeholders#editors) update the draft data model based on information collected in `step 14`, `step 15`, `step 16` and `step 17`. 

<details>
  <summary><b>Description</b></summary>
  The draft data model expressed as an UML diagram with textual description (i.e. tables) of the entities, attributes, relationships, definitions and cardinalities is updated. The editor constructs the new version of the data model based on the changes that have been agreed upon and derived from the previous four steps.  
</details>

<details>
  <summary><b>Rules and Guidelines</b></summary>
  
Publication as a Working Draft does not imply endorsement by the Working Group members or its representatives. This is a draft model and may be updated, replaced or made obsolete by other model at any time. It is inappropriate to cite this model as other than work in progress. 
</details>
