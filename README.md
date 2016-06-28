# HealthTranslator-Corpus
A Portuguese corpus of 38 documents with medical concepts annotated. This corpus was created and used to evaluate concept coverage of [HealthTranslator](https://hugosousa.github.io/HealthTranslatorClient/) but is open access and may be used for any other purposes.

Laypeople and health professionals were asked to annotate medical concepts in a collection of documents. Generally, laypeople should be able to perform a good quality annotation of medical concepts. Even though they might not know the definition of a concept, they should be recognizable by its knowledge and context. Moreover, about half of the `laypeople' invited to annotate the documents are not really lay to the subject as they are currently finishing health-related courses, such as nursing or medicine.

Ten people were invited to constitute the lay group as they have a bachelor or superior grade. Moreover, six of them are currently finishing or working in health related areas, such as nursing or medicine. The professional group is composed of six nurses and doctors. All of the invited people have sufficient skills to perform the annotation tasks in the chosen tool. 

Although initially the goal was to create a collection of 60 documents, inviting professionals such as doctors or nurses to annotate the documents was a hard task and only 38 documents were successfully annotated by this group. The documents were gathered and classified as belonging to the medical domain by a [crawler](http://nlp.ilsp.gr/redmine/projects/ilsp-fc) and are available for [download](http://qt21.metashare.ilsp.gr/repository/browse/qtlp-portuguese-corpus-for-the-medical-domain/27c3e8aa6bdb11e3b61300155dbc02019a678f0685874a03a2aa35640f92b204/).


The process was split in 2 phases. 
The first phase consisted in providing documents to be annotated by each person. 
The crawler removes boilerplate of the documents and, for each sentence, presents concepts automatically detected. These concepts were initially automatically annotated as they might help the users and reduce the time needed for the annotation task. However, users must remove them if they feel these concepts are incorrectly recognized. 
Annotators were given guidelines in order to provide a consistent annotation among different people. For example, there should be no nested concepts, as the most specific term should be annotated.

The same document was independently annotated by a person in the "laypeople" group and another person in the "professional" group.
The documents of a person do not match all the documents of another person. 
This task was done in [egas](https://demo.bmd-software.com/egas/tool/), an annotating tool able to export annotations in [brat standoff format](http://brat.nlplab.org/standoff.html), also known as A1.

Later on, the terms that were annotated by the person in a group, but not by the corresponding person in the other group were sent to the latter, in order to disambiguate terms that might have been forgotten and create an agreement corpus. For example, if an annotator of the professional group identified the term `hypertension' and the corresponding annotator in the lay group does not, this term was sent for revision to the layperson, which then decides if he agrees it is a medical concept or not. 

Therefore, the gold standard corpus is the group of documents with annotations composed by the consensual concepts on both sides.  Although the lay group completed both annotation phases in 60 documents, only 38 documents were finished by the professional group. Thus, this corpus is constituted of 38 documents with a match on both groups, but there are 22 documents annotated by laypeople but without a matching professional annotation.

Note: The annotator's identity have been anonimated. Thus, persons from the professional group are represented by a letter and from the lay group by a number.
