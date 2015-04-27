# Programme (strand) Update #
_**Please note: if you would like to do further searches across all the jiscEXPO project blogs please use this [jiscEXPO Search Engine](http://www.google.co.uk/cse/home?cx=008736370747590052728:tpsy-szje3k) which works well alongside reading this report if you want to dig into further advice and guidance.**_

Sections in this report:
  1. Change: where has progress been made by the projects in this programme? #eval-change
    * Changes that have happened
    * Changes that have not happened
    * Anticipated changes
    * Gaps
  1. Shared Lessons / Products: what lessons and/or products from the programme could be shared with other projects/programmes? #eval-products
    * Soft (intangible) products
    * Hard (tangible) products
  1. Risk: what previous risks were identified and what mitigations were put in place? #eval-risk
  1. Stakeholders: what are the most important relationships? #eval-stakeholder
  1. Milestones: what key milestones do you expect over the next quarter? #eval-milestone
  1. Spend: What is the current and predicated spends of this programme? #eval-spend
  1. Conclusion & recommendations: What key message should be told about this programme to the sector?

## Change: where has progress been made by the projects in this programme? ##
The change described in this section is building on the Programme Definition, aka [Programme FAQ](http://code.google.com/p/jiscexpo/#FAQ).

### Changes that have happened ###
All of the #jiscEXPO projects were required to a.) expose linked open data, and b.) build a prototype on the linkeddata that made it valuable to an end user.  The importance of exposing linkeddata is best outlined by the inventor of the Web in his talk about "The 5 Stars of Linkeddata".  While this original "5 stars" talk was focused at government departments and asking them "how many stars their website provided in terms of being transparent and open"; this question also rings true for University web sites in terms of influencing Web Managers as they do not want to be managers of web sites that are 1 or 2 stars as it implies this is equivalent to staying at a hotel with 1 or 2 stars.  Of course achieving a 5 star rating is not a trivial task and requires real resources to achieve.

  * All #jiscEXPO projects have data exposed now, all with a 4 to 5 star rating.
    * Announcement of the exposing of the BL's British National Bibliographic dataset: http://openbiblio.net/2010/11/22/querying-the-british-national-bibliography/
    * Announcement of the first data.INSTITUTION.ac.uk website at the Open University: http://www.data.open.ac.uk
    * 12.1 million pages of RDFa on music data released: http://linkedbrainz.c4dmpresents.org/content/how-many-musicbrainz-pages-will-have-rdfa
    * There are various technical expose methods which can broadly be categorised as: triplestore SPARQL endpoint, RDFa embedded in html5/xhtml, serialised RDF as a ReST interface, nosql stores such as mongoDB, voldermort and redis <-- please use the [jiscEXPO Search Engine](http://www.google.co.uk/cse/home?cx=008736370747590052728:tpsy-szje3k) to search for examples

**_The process of exposing linkeddata was not a trivial one and required new methods, tools and skills to transform the data in its various states into a common structure._**

Perhaps first and foremost was the importance of learning how to work as a team with the new linkeddata paradigm.  The methodology adopted usually revolved around the tools, but also required that careful consideration be made for the processes that were used to collect data from various people both in and outside the institution.  Everyone from caterers, estate managers, librarians, marketing teams, researchers, lecturers, students, corporate developer teams, volunteer communities and many more were approached for use of their data.  Once permission were agreed, the team had to then utilise existing tools or write their own tools to work with the data:

  * All projects commented on the methodologies for exposing and streamlining the processes of exposing linkeddata, exemplars include:
    * XML to RDF streamlining and validation checking:
      * http://lucero-project.info/lb/2010/08/initial-overview-of-the-lucero-workflow/
      * http://blogs.ukoln.ac.uk/locah/2010/08/18/some-thoughts-on-architecture-and-workflows/
    * Overall vision and diagram for how the data would be repurposed for end users: http://code.google.com/p/jiscexpo/wiki/fishdlish#From_with_#fishdlish #fishdlish
    * Use of project methodology "agile scrum" to get data exposed: http://chalice.blogs.edina.ac.uk/2010/10/18/musings-on-the-first-chalice-scrum/
    * Satirical post on the differing approaches for modelling data: http://blogs.ecs.soton.ac.uk/webteam/2010/09/02/the-modeler/

While collecting and exposing large sets of data are what the jiscEXPO projects are primarily engaged in doing (many of them using large triplestore-databases), there have also been several smaller experiments with how to transform smaller datasets into linkeddata.  This is a significant hurdle to overcome as -at the end of the day- human users usually input data using things like wordprocessing and spreadsheet tools at a micro data level (not a macro data level - which is usually what machines do).  For humans, being able to take a small bit of data and work with it for specific needs is where many end users who have basic computer literacy skills could benefit from linkeddata, i.e. being able to download a subset of data from a large datastore and then work with it as a single spreadsheet of data.  Many researchers could obviously benefit by working with data in the raw which is a key user group for several of the projects.

  * Tools for exposing linkeddata:
    * Google Refine is a spreadsheet-like power tool that enables data to be downloaded and worked with at a bespoke level: http://ldfocus.blogs.edina.ac.uk/2011/02/25/institutional-locations-as-linked-data-through-google-refine/
    * ePrints RDF export for bibliographic resources: http://lucero-project.info/lb/2010/11/publishing-oro-as-linked-data/
    * Use of Open Provenance model to join bibliographic records: http://openbiblio.net/2010/09/22/disambiguation-deduplication-and-ideals/
    * Using Linkeddata with Android for a Samsung Galaxy TV: http://www.greenhughes.com/content/using-linked-data-app-inventor-android-help-bridging-script
    * Review of linkeddata browsers: http://fishdelish.cs.man.ac.uk/2010/first-fishing-expedition/ <-- also see series of "fishing expedition" posts
    * Deciding which triplestores to use: http://fishdelish.cs.man.ac.uk/2011/triplestores-looking-back/
    * Working with D2R to convert datasets into triples: http://linkedbrainz.c4dmpresents.org/content/adventures-ad-hoc-rdfa-development-musicbrainz
    * Open Org Grinder is a tool serialising Organisational Structures: http://openorg.ecs.soton.ac.uk/wiki/OpenOrg_Grinder
    * Please use the [jiscGEO Search Engine](http://www.google.co.uk/cse/home?cx=008736370747590052728:tpsy-szje3k) for further examples.

Potentially the most significant advancement in terms of innovation curve were the skills achieved by the projects.  Best of all these skills are now being passed on to other people in the Academic sector.
  * Skills for exposing linkeddata as RDFa: http://linkedbrainz.c4dmpresents.org/content/adventures-ad-hoc-rdfa-development-musicbrainz
  * Developer transformation into a linkeddata developer: http://lucero-project.info/lb/2010/12/putting-linked-data-to-work-a-developers-perspective/
  * Recognising a large learning curve for linkeddata at first but then levels out and returns back the value: http://blogs.ukoln.ac.uk/locah/2010/12/01/assessing-linked-data/
  * Learning and documenting use of SPARQL queries: http://fishdelish.cs.man.ac.uk/2010/progress-2nd-december-2010/
  * How to do data triage (aka beating data into shape so you can work with it): http://openbiblio.net/2010/09/22/data-triage-notes/

While technical skills (because of the tools used to do the heavy lifting of the large data sets) are the bulk of skills being developed in the project there are also very real philosophical skills needed in terms of being able to think about vocabularies, authority files, taxonomies and URI sets.  The skills of data modelling as well as ontology creation are essential logical reasoning skills that are required for all of these projects.

  * Issues and concerns around reusing & modelling vocabularies and terms (aka ontology predicates): http://blogs.ukoln.ac.uk/locah/2011/03/08/describing-the-things-the-rdf-terms-used-part-1/ #locah
  * Deciding how to model music composer data over the years to encapsulate composers from Bach to the Beetles: http://musicnet.mspace.fm/blog/2011/01/19/musicnet-uri-scheme-and-linked-data-hosting/ #musicnet
  * On initial startup concerns for people in having to use that part of their brain that requires ontological reasoning: http://ldfocus.blogs.edina.ac.uk/2011/02/23/episode-1-universities-colleges-and-their-services/ #ldfocus
    * Discussion on the usability of selecting which terms to use while using authoring tools https://opencitations.wordpress.com/2011/02/25/using-cito-in-wordpress/  #jiscopencite
    * Rapid prototyping your data modelling diagram: http://ldfocus.blogs.edina.ac.uk/2011/03/03/introduction-diagram/

Note: having comments on "IPR" in the last programme update report (and also again below), I'll just leave a note that all projects have had to undergo a process of licensing the data in a more transparent and easily moveable manner than is allowed even by partially open licensing like CC-attribution.  Most projects had to make a decision in terms of an completely non restrictive license like CC-zero or PPDR.

### Unexpected changes ###
All projects must deal with the problem of sustainability, and with linkeddata this problem is amplified as if the URIs created by the projects for their data are not kept around in the long term then as other linkeddata projects build on the previous set of URIs from the last project there is a dependency created for sustainable URIs.  This was addressed right from the start of the programme by several projects.  An emergent response to this by projects was the community talking about the need for a central data.ac.uk to act as a place to store URIs in the long term.  However, the political implications of a central data warehouse for the academic sector, like that of data.gov for the government sector is much slower moving in terms of being set up.  Parallel to the call for a data.ac.uk was the
  * Original call for a data.ac.uk website for the Academic sector http://musicnet.mspace.fm/blog/2010/07/20/data-ac-uk-proposal/
  * Concerns for most appropriate place for data that is shared by the sector: http://sailsproject.cerch.kcl.ac.uk/2010/12/where-should-the-data-go/

The W3C also recognised the significance of linkeddata as well as the growing amount of Bibliographic metadata becoming available as linkeddata, the 'linkeddata in libraries' working group began to collect use cases of which a couple of jiscEXPO projects had use cases collected from them.
  * http://www.w3.org/2005/Incubator/lld/wiki/UseCases

### Changes that have not happened ###
All changes have happened as predicted, I'm a psychic oracle! 8D - that or I didn't over promise our capabilities for change at the start ;-)  - "The only change management principle you can scientifically apply is that Disruptive Innovation is always just hiding around the next corner."

### Anticipated changes ###
It is the final output from the projects that we are waiting for with bated breath.  We have started to see some soft product launched (alpha prototypes) that helped expose the linkeddata (and potentially could be reused by developers).  However, the key to the final product prototypes is that they focus on being useful to real end user needs.  In short we are hoping that we will see two or three visionary prototypes that will inspire others in the Academic sector (especially managers and other budget holders) into investing towards the future potential that the visionary prototype is able to demonstrate.

## Shared Products / Lessons: what lessons and/or products from the programme could be shared with others in Academia? ##
The next two sections cover soft (intangible) and hard (tangigle) products that have been produced thus far.  These products are not necessarily ready for use by end users but rather are in an alpha testing stage and should be see as extremely bug prone and likely to crash.

### Soft (intangible) products ###
Soft products are the things like skills, relationships, ways of working and user experiences from the project that have enabled innovation.

  * Licensing and understanding the importance of licensing on the Web as it pertains to linkeddata: http://lucero-project.info/lb/2010/11/publishing-oro-as-linked-data/
  * Principles for Open Bibliographic Data: http://openbiblio.net/2011/01/20/open-bibliographic-principles-announced/
  * Suggested URI patterns for a bibliography service: http://openbiblio.net/2010/10/26/some-obvious-uri-patterns-for-a-service/
  * Using student transcribers to encode linkeddata of natural language texts: http://sailsproject.cerch.kcl.ac.uk/2010/12/student-transcribers/
  * Understanding how to work with RDFa for developers: http://linkedbrainz.c4dmpresents.org/content/adventures-ad-hoc-rdfa-development-musicbrainz
  * A suggested namespace pattern for places: http://chalice.blogs.edina.ac.uk/2010/11/10/structuring-a-linked-data-namespace-for-places/

### Hard (tangible) products ###
Hard products are things like software apps, guidance reports, policy/process frameworks and other items that can be passed on to other people for reuse.
  * As mentioned above the potential for Universities to share their data using a data.foo.ac.uk URI syntax so anyone (either inside or outside the institution) can know where the common village data watering pump is:
    * data.open.ac.uk
    * data.southampton.ac.uk
    * Plans by King's for a data.kcl.ac.uk: http://sailsproject.cerch.kcl.ac.uk/2010/12/where-should-the-data-go/
  * A tool for documenting how to write SPARQL queries: http://fishdelish.cs.man.ac.uk/idoc/page/first-fishing-expedition-reboot
  * A tool for visualising ontologies: https://opencitations.wordpress.com/2011/02/25/using-lode-for-ontology-visualization/
  * A set of vocabularies for describing all the things to do with research publications: http://opencitations.wordpress.com/2010/10/14/introducing-the-semantic-publishing-and-referencing-spar-ontologies/
  * Software library for bulk bashing data from multiple endpoints: http://openbiblio.net/2010/09/09/introducing-ofs-a-python-bucketobject-storage-library/
  * Proposed vocabulary modelling of the 'Encoded Archival Description' (EAD): http://blogs.ukoln.ac.uk/locah/2010/09/28/model-a-first-cut/
  * URI schema for music composers: http://musicnet.mspace.fm/blog/2011/01/19/musicnet-uri-scheme-and-linked-data-hosting/
  * Search engine for finding music composer URIs: http://musicnet.mspace.fm/blog/2010/06/22/project-timeline-workplan-methodology/
  * A tool for subject experts to use to match term names with sameAs terms names: http://musicnet.mspace.fm/blog/2010/10/19/alignment-tool-implementation/

## Risk: what previous risks were identified and what mitigations were put in place? ##

Ongoing concerns around the longevity of URIs, especially as apps and tools are built atop these datasets.
  * mitigation: currently pursuing a central data.ac.uk website where these things can be stored.

The delivery of the visionary prototypes by projects is one of the key aspects for pushing forward linkeddata as an interoperable technology, if these prototypes do not clearly meet end user needs (where senior manager's can easily see their value) their is a risk for the advanced technology behind the scenes not being recognised as valuable.
  * mitigation: contacting projects reminding them of the Call aim as well as bringing together a panel of outside user experts to evaluate the prototypes and provide guidance on their presentability and likeability. Call for this same focus at the ISWC keynote speaker: http://iswc2010.semanticweb.org/node/80


  * how to model data... the old way to create vocabularies (database schemas) vs the new URI is the thing
    * data spam - provenance.
    * understanding the difference between spreadsheet data and wordprocessing data: http://openbiblio.net/2010/11/18/characterising-the-british-library-bibliographic-dataset/

The value of linkeddata as a technology is widely recognised but the business case for linkeddata is still to be determined.  Will it save money, will it enable new innovations, will it do what it has promised?  JISC must consider these risks if it is going to proceed with supporting innovation work with linkeddata at the core.  Most importantly, the user must come first not the technology and so a readjustment must occur putting the humans in front of the technology.
  * mitigation: in planning the future set of work for linkeddata we've started to look at the social implicaitons
    * business case - 5 starts of LD
    * see focus on usability rather than tech. <-- Semantic Social Scholarly Infrastructure #jiscSSSI
    * 

The Big Data problem.  Perhaps the most significant potential for linkeddata is to think bigger than anyone has ever thought possible in terms of helping organise Big Data (aka finding the needles in the planet sized haystacks). Companies who were leaders in the internet early days are starting to see massive sets of data (petabyte --> exabytes --> zettabytes --> yotabytes...), eBay and Amazon have user activity data in the exabytes.  Likewise the production of data in research facilities such as at CERN or even by the likes of electron microscopes have the potential of providing more data in a day than a human could read in a lifetime.  Machines being able to accurately process and interpret this data for humans is essential.
  * mitigtation: JISC had a reporter sent to the O'Reilly Big Data Conference (Strata) and had the report sent around to all the projects to be read by and considered in correlation with their own projects: http://cottagelabs.com/strata-2011-review/


## Stakeholders: what are the most important relationships? ##

Organisations:
  * data.gov.uk
  * British Library, see linkeddata in libraries report:
  * BBC
  * Europeana:
  * Open Knowledge Foundation
  * OCLC

Academic Sector:
  * UCISA
  * Sconul
  * RLUK
  * UK Archives Discovery Network

User groups / types:
  * Developers
  * Information professionals
  * Head of ICT
  * scuba divers,
  * Name place authority community

## Milestones: what key milestones do you expect over the next quarter? ##

Project/Programme Milestones:
  * Projects alpha release of products
  * Final Newsletter from PEG
  * Project end dates
  * Final Programme Meeting
  * Programme product review panel
  * Final report and presentation from PEG
  * Linkeddata

Events:
  * Linkeddata Hackdays at Bristol
  * dev8D
  * MusicNet workshop
  * CNI 1st April 2011 in San Diego, CA, USA
  * LOD-LAM in San Francisco 19 May 2011
  * Open Repositories in Texas 7 June 2011
  * OAI7 in Geneva 22nd June 2011
  * BNCOD2011 12th July 2011
    * jiscEXPO Programme Meeting
  * Linkeddata Camp at LoC (after Socety of American Archivists) - 25 Aug 2011

## Spend: What are the projected spends of this programme? ##

  * Total projected spend for 12 projects: £850k <-- mostly spent and all committed, pending any project underspends.
  * Programme Evidence Gatherer (aka Synthesis Liaison): £13k <-- committed.
  * Programme Meeting: £20k <-- estimated cost.
  * Synthesis & Commissioned Reports: £2k (Strata Big Data Report) + linkeddata guide? <-- this cost could increase with additional lessons learned guide on linkeddata?

Estimated Total: <£885k

# Conclusion: What key message should be told about this programme to the sector? #

Learning about linkeddata makes you a better person: or at least makes you better at your job. Whether you are a developer, librarian, information professional, teacher or researcher - the skills around understanding the way you organise data (e.g. your files, folder on your computer desktop, the vocabularies/taxonomies your subject area uses, etc) is an essential skill that all humans will need to have in the future to take advantage of the things that computers can do for them.  Computers must operate using logical structures and the more logical structures we put online and label with web addressable URIs will assure that machines can do more work for us in terms of organising, discovering, disseminating and transforming data.

1.) Cost savings in metadata management across the sector, i.e. bibliography metadata is becoming cheaper to reuse across disparate systems.

2.) Efficiency for managing institutional management data for reuse across the institution, e.g. data.ac.uk efforts, also especially ease of basic users being able to make their data reusable like catering data at

3.) Global wide use of 'big data' research datasets where thousands of researchers are using for producing research, i.e. music data, DNA data, astrological data, etc.

## Quotes: ##

  * "Linked Data is part of an idea to move to a “web of data” from a “web of documents”... For me this fitted very well with another big change happening in the web; the move away from just looking at web pages on a desktop computer to consuming data on lots of other devices like mobiles, smart televisions and tablets... so my experiments so far have centred around the idea of bringing OU data into new contexts such as mobiles and to the social web."
  * "Also if two sites support a Linked Data endpoint the way you work with them will be broadly the same, you don’t have to worry about things like downloading any extra software libraries to be able to access the API."
  * re SPARQL - "...data you can return is very flexible, you don’t need to look up the syntax of a new API call every time you want new information"
  * "With Linked Data this more rigorous modelling is more exposed and up-front"
  * "I found that there simply wasn’t enough helpful information about how to create a data model. This would have saved me quite a bit of time because I think the data model is so central to what we are doing and provides such an effective way to visualise the entities and relationships between them..."