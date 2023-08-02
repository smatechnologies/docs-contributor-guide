# Best Practices

This page will highlight Best Practices for User Experience standardization and collation of Education products including Training and Documentation.

Excepting specific circumstances and needs, which should be verified with the Education department, all documentation should be written using **Markdown** syntax.

## Text Standardization for English Language Materials

* File and Folder Names - no capitals, no spaces (avoid Camel Case)
    * If a space is required, it should be hyphenated
* Table of Contents and Navigation (Headings) - All Capitals excepting articles


## Organization

* Put the most important details and information at the beginning and include additional information (only as necessary) at the end of the document.

* Use appropriate breaks for ease of reading. Avoid large walls of texts.
    * Subheadings can be useful to create visually pleasing and sensical breaks.

* Use Headings and Subheadings to create a hierarchy of information for each page. Using **Header 1**, **Header 2**, and **Header 3** will create a right-panel submenu on the page.

* Reserve **Header 1** for page titles.

* Provide instructions in step-by-step, numeric list format.

## Language and Grammar

* Write your documentation in second person, present tense using instructive (active) voice.

:::tip Example
    
* Click the **Next** button
* You should see a pop-up box to the left
* Restart the LSAM

:::

* Summaries should be clear, simple, and concise. In documentation, avoid describing **why**. Focus on documenting **what** and **when** it does something.

* Limit technical jargon to specific needs concerning the product. If acronyms and abbreviations are used, they should be defined and explained in the first instance of the usage.

* Use consistent terminology - avoid using multiple spellings or differing references to the same content
    * **Self Service** vs **Self-Service**
    * **UNIX** vs **Unix**

* Content detail should be written as complete sentences. An exception is in the use of header summaries, which are intended as file “titles” more than sentences.

* The Oxford (or serial) comma provides clarity in all situations and should be implemented when listing elements in summaries, descriptions, and parameter or return descriptions.

* Avoid contractions

## Lists vs Tables

* Within Docusaurus: 
    * Tables should be used for technical lists that use only a few words or phrases in each section
    * Lists should be used when any section requires a description with **more** than 2-3\* sentences 
        * Lists can use **Header 2** or **Header 3** to create or add to the right-panel submenu

\*Aesthetic discretion can be used to determine whether a list or table should be used

## Admonitions in Docusaurus

See example syntax here: [Admonitions | Docusaurus](https://docusaurus.io/docs/next/markdown-features/admonitions)

* Best practice for Admonitions is to include a space between both sides of the fencing and the admonition text as seen below.

**Tip** and **Example** use *tip* (green) admonition format to illustrate “How-to” information. For example, a tip on navigation shortcuts  or examples that illustration “how-to” utilize or implement an OpCon object or concept.

```

:::tip

This is an example of the Tip syntax with a **Tip** Header

:::

---

:::tip Example

This is an example of the Tip syntax with an **Example** Header

:::

```

:::tip 

This is an example of the Tip syntax with a **Tip** Header 

:::

---

:::tip Example

This is an example of the Tip syntax with an **Example** Header

:::

* The **info** (blue) admonition should be used to identify topics of special notice that do not fall under the category of Example or Tip but should be highlighted. For example, a version-change based behavior or specialized knowledge or data specific to a content topic.

* The **caution** (yellow) admonition should be used to identify activities or changes that require special steps or understanding for clarification. For example, calendar changes or time zone naming and offsets that can affect scheduling.

* The **danger** (red) admonition should be reserved for activities or changes that are breaking in nature.

* The **note** (white) admonition may be avoided for stylistic purposes and replaced with the info admonition.

## Media

* Use images and diagrams sparingly.
    * Images should enhace the textual documentation, not replace it.

* Images and diagams should be used to: 
    * Guide users through a complex procedure
    * Show high information windows or screens
    * Add clarity to workflows and configurations
    * Provide visualization of a process
    

* Use markdown formatting for inserting images.



## Inclusive Documentation

In briefest terms, our documentation should be written with inclusivity and diversity in mind.

* Avoid ableist language, unnecessarily gendered language, unnecessarily violent language.

* When appropriate, replace established terms that reflect bias with more inclusive language.
    * If established technical language is recongnized as harmful but cannot be replaced, always write the terminology within code fencing font.

## Attribution 

* Refrain from copying and pasting material that does not belong to SMA Technologies to avoid Intellectual Property or Copyright conflicts.

* If external material must be referenced, always provide a direct link to the source material.




