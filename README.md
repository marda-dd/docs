# MaRDA Data Dictionaries Working Group

## Motivation

Shared datasets often have column/field names that are ambiguous in their meaning, or contain identical/related concepts with different names, hindering reuse. For example in electron microscopy, "high-tension" and "acceleration voltage" are used interchangeably (identical concepts, different names). However, "magnification" and "field-of-view" are not the same thing, but are closely related (domain experts know that dividing the field-of-view by pixel size will return the magnification value). This ambiguity happens regardless of the method of sharing -- via files, web pages, or APIs. The traditional solution for this is to provide documentation.

However, documentation is typically delivered “out-of-band”, i.e., not directly linked within the same artifact (file/object) as the data. Thus, a data consumer needs to link terms to their definitions by eye, i.e., one reads many pages of documentation based on one’s needs, creates an ontological map in one’s mind that must be re-created again and again (which should best be replaced by a machine accessible ontological map) - which raises the barrier to data reusability. Furthermore, any linking among terms by different data providers, whether to assert equivalence or to clarify differences, is typically done in an ad hoc manner, hindering interoperability and thus reuse.

## Work Plan

This working group will produce a Working Group Note<sup>[1](#fn1)</sup> for sharing materials research data as [5-Star Linked Data](https://www.w3.org/DesignIssues/LinkedData). Specifically, the working group will:
1. run a pilot study using datasets from three (3) independent materials research data providers. The working group will split into three interdependent groups, one per dataset, to ensure:

    - (a) a data dictionary is created and deployed online, with resolvable HTTP URLs for each term, that documents the fields of the dataset;
    - (b) the dictionary for each dataset includes qualified links to terms of another dataset’s dictionary. In the cases where terms are related but not equivalent, those relationships are explained and documented; and
    - (c) the dataset itself is made accessible as Linked Data, and thus self-describing in linking to its data dictionary.

2. produce a Working Group Note that uses the completed pilot study as a case study in order to document learnings in (a) creating and deploying a data dictionary for a materials research dataset; (b) relating a dictionary’s terms to external terms in order to provide richer context for a data consumer; and (c) producing a self-describing distribution of a dataset by linking to its data dictionary.

Proposed timeline (12 months): Six months for Activity 1 (Pilot study), with two months allocated per sub-activity (isolated data dictionaries, linked data dictionaries, and linked data). A further six months to produce the Working Group Note (rounds of Working Drafts, iterating on pilot study activities, etc.).

<a name="fn1">1</a>: Terminology references the [W3C Process](https://www.w3.org/2004/02/Process-20040205/tr.html). While the produced Working Group Note may later advance in maturity level towards e.g. a Candidate Recommendation, the scope of this working group is to produce a demonstrative technical report.
