# How I Explained Linkeddata to a Librarian #

_One day I fell asleep at my desk and had an almost hallucinogenic dream where I had a conversation with Melville Dewey (the inventor of the Dewey Decimal System), the follow is my recollection of that dream_

Flanders: Wow, Melville Dewey what are you doing visiting me in the 22nd century?

Dewey: Thanks to a crack in the space-time continuum (due to me understanding of the metric system) I've been able to travel forward in time to observe what is becoming of my decimal system for books.

Flanders: Cool, so why are you talking to me?

Dewey: I can only visit people born on December 10th and you seem to be the most enlightened with regards to the latest that has been happening on this thing called "the Web" (not a lot of people have updated their bios for me to look up their birthdate - something about data protection?)!

Flanders: I'm honoured, so what can I tell you... or rather more importantly when was the last time you checked in to see what was happening?

Dewey: Last I checked in, was with Howard Martin Temin who while an interesting scientist really didn't have much to say other than it was easier to get his books on the shelf thanks to the MARC format.

Flanders: Wow, yes things have moved on a bit thanks to the Web.

Dewey; What's the Web?

Flanders:

Flanders: The inventor of the Web!

Dewey: How do you invent the Web?

Flanders: Well he invented the HTTP protocol and the first servers that it ran upon.

Dewey:

> structured data is any kind of data that a machine can read, linkeddata is a more specific type of structured data that is "self describing".  The simple example being something like a MARC record where I can show a librarian this:

"100 : J.K. Rowling"

A human can read the above if they know MARC, but a machine cannot read it unless you load the MARC "language" into it the machine's "brain" so it can dereference the "100" and know that "100 = author name".  So MARC (as its acronym implies) is "Machine Readable" and therefore it is "structured data", however it is not "self describing" and therefore is not linkeddata.  So how can you enable data to be machine readable without actually having a human load a special vocabulary language like MARC so the machine can read it?  Back to our MARC example: a human might not know what MARC "100" is (if you are not a librarian), but in this day and age you can just go and look up "MARC 100" on Google and find out pretty quickly (after looking at the first 4 or 5 results on Google).  Machines can't do this as they are bad at reading our language.  Rather we have to give machines the capability to look up things on the web, like us using Google: this is what linkeddata is all about.  Instead of a machine going and searching for "MARC 100" on Gogole we need to have something more specific for the machine so it doesn't get confused (in fact the killer question for any structured data is "how much do we need to disambiguate in our own human language for machines so they can help us more?), instead we need to be able to say to machines this is **exactly** what I mean when I use the term "MARC 100", linkeddata of course suggests that you use "links" instead of "human terms".  So by changing "MARC 100" to be a be more specific and **self describing** we can make the "100" an exact link which the machine can understand, so I've made up this link for MARC 100:

http://bl.uk/vocabulary/MARC/100

Of course, there are lots of politics around who should own what "links" and what you should do when you have duplicate links, so for example if the LoC decided to create a link that is the same as the BL's link:

http://loc.gov/vocabulary/MARC/100

Either of these links can be "read" by machines and because they are specific links the machine can then go and look at these pages and automatically know what is being "said" to it.  This is therefore "self-describing data" as the machine, like us, when it gets confused can just go and "ask" the Web for the answer.  This is linkeddata (more of less).

--> 2. What is the difference between using linked data or APIs and is one easier to do than the other?

--> This is a more difficult question as linkeddata is not an API.  Rather linkeddata is like a philosophy and there are numerous philosophies on the Web (remember the Web is NOT a science!) and so things like religion and philosophy are VERY important as it is about getting the masses to **believe** in the way you think the Web should work.  To contrast 'linkeddata' with the most popular philosophy on the Web right now, you could look up ReST based architectures, coincidentally people who 'believe' in ReST are called ReSTifarians which in itself somewhat describes their outlook on the Web.  One of my favourite (though perhaps somewhat patronising) explanation on ReST is here:

http://tomayko.com/writings/rest-to-my-wife

So in comparison 'linkeddata' as a philosophy (or religion) is advocating a certain world view about the way we should **design** the plumbing of the Web (which is what APIs are: plumbing to get data through pipes). However, unlike 'ReST', 'linkeddata' is trying to talk more about fine grained data, i.e. things smaller than a "Resource", so my example above re having a single HTTP link for a single term in the MARC vocabulary (bl.uk/vocabulary/MARC/100) is not a "resource" but rather it is a data element in a vocabulary (NB the "vocabulary" is more the type and size of things that we humans -and ReSTifarians- would call "a resource", in fact I can point to the resource that is the 'MARC vocabulary resource' with this link, yet there are not additional links within this link to make it linkeddata: http://en.wikipedia.org/wiki/MARC_standards).

Therefore, linkeddata is trying to talk about a different set of things on the Web that most people would call "datasets", where ReST is trying to talk about the way you do things with "resources".  An easy way to think of the difference between the two (though not completely accurate) is that ReST is generally philosophising about anything that you would create with a Microsoft Office Word document (e.g. essays, books, tweets, blogs, reports, articles, etc - i.e. "natural language text"), while linkeddata is philosophising about how to do things with anything you would create with a Microsoft Office Excel document (e.g. spreadsheets, databases, graphs, lists, vocabularies, thesauri, key-value pairs, etc).

In short, linkeddata is obviously trying to be more specific about granular pieces of information, where ReST prefers to be more generic.  I'd reference or chat on the phone with regards to "how specific do we need to be for a machine to wash a plate for us" - do the machine need to know the color, size, viscosity and material of the plate or does it just need to know that the plate is 'generally' this size and shape?  Linkeddata is trying to ask the more specific questions about the 'plate', where ReST is fine with it being a bit more fuzzy and generic.  Of course the nice thing on the Web is that the religions that people have around philosophies like ReST, Linkeddata, Web Services, Enterprise Architecture and the rest are not incompatible (this is more like trying to agree a common ground between Buddhism and Zen philosophy than trying to meld Christianity and Muslim beliefs - though the flame wars between the two sides often seem like it is the latter not the former, NB the all male developer crowd does not help this).

Ok so with that knowledge in the foreground I'll try and better answer your question. In short, currently using an API built using a ReST philosophy is MUCH easier than using an API built with a linkeddata philosophy.  However ReST doesn't have the capability to do more things than they was we currently use the Web, so to go back to the washing machine analogy, if ReST is the current day washing machine then it it does it's job, but if we wanted a washing machine that could not only clean the dishes but then also pick them up and put them away in a cabinet according to their size or type then we would need linkeddata.

So my involvement in linkeddata can be summed up by the following quote:

"I'm an inventor.  I became interested in long term trends because an invention has to make sense in the world in which it is finished, not in the world in which it is started." - Ray Kurzweil