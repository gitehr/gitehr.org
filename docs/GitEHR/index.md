# GitEHR

GitEHR is a decentralised and portable health record, powered by Git, cryptography, and open standards.

## Databases Considered Harmful

Since I began working in health technology over ten years ago, I've constantly struggled with how we can make a health record that is interoperable and portable.

Much work is already out there on health interoperability, and I have finally, and sadly, come to the conclusion that it's **all** misguided. Adoption of databases for the content of the health record was the wrong path and has resulted in total chaos across health tech, vast sums of wasted money, and records which are not in any way interoperable.

Traditional health ineroperability focuses on sending data from one **Organisation-Centric Database** to a different **Organisation-Centric Database**. 

Looking at examples from other parts of the tech world, there are no successful examples of that approach working at scale. What does work is sending files. Distributed Version Control Software such as Git provides an excellent example of how to engineer multi-contributor, secure, private repositories which are agnostic of the software being used to view and manipulate them.

Throughout my health informatics career, I've tried to learn as much as possible about how existing solutions in technology could be applied to the health tech space. We don't always need to do our own health-specific thing. Many of the problems we see in health tech are already solved in the wider tech world, hence GitEHR draws extensively on existing technology. There might be areas where we do need a healthcare-specialised technology, but the majority will use tried and tested existing software.

!!! quote "Rob Dyke Says"
    "All software has already been written"

## Databases are Organisation-centric By Definition

When you build a system which uses a database, it's hard to go to all the effort of creating the database and then use it for one patient. You could, but nobody is going to do this, because part of the point of having a database is to aggregate and index data across your whole organisation.

Databases work fine within the walls of *your* organisation.

But the problem comes when you try to interoperate this database with *other* databases at *other* organisations. Even where organisations have the exact same EHR deployed, the local deployment customisations that have inevitably been made make it hard (if not impossible) to move data around. If you *can* move data, there is usually some work involved in 'translating' the data from one database to another. And this has to be done between every single organisation and for every item of data. This rapidly becomes unworkable.

Some people think the solution to this is simply to make the databases **BIGGER**. But that just moves the problem rather than solving it. You simply trade local inter-organisational interoperability problems for different and harder problems at regional, national, or international, (or interplanetary) scale.

We have to change the paradigm, and I think GitEHR is the start of the road for that change.

We need an interoperable and extensible file format for medical records. It will be an open standard and the reference implementation will be open source. Many other implementations can exist. Many platforms for the reading, writing, and processing of these records can exist.

It will solve the problem of interoperability and will make a start on solving many other unsolved problems of health technology.

