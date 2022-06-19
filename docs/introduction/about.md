# About GitEHR

GitEHR is the product of over a decade of learning and thought within the health technology industry, trying to find a solution for a life-long clinical record which is inherently patient-centric and did not have the interoperability problems of other types of health record.

## The story of GitEHR

As a clinician starting to become interested in health tech in ~2011, just as the National Project for IT (NPfIT) was collapsing, I found it really difficult to find a 'way in' to the world of GP IT. Clinicians, it seemed, were not wanted, in a world which was dominated by large companies delivering software which was unusable and 'legacy' from day one.

Eventually I found two ways in: NHS Hack Day, and the RCGP Health Informatics Group. These were my starting points, but since then I've been almost full-time in health informatics, in a range of roles from the unorthodox: freelance General Hacktitioner to the very much orthodox: Chair of the RCGP Health Informatics Group (HIG)

I've had a somewhat unusual Clinical Informatics career in that I've also learned a lot about the **technical** underpinnings of the software. Unlike many clinicial informaticians and NHS digerati, I learned to write code and become deeply technical, giving me a different way to view the proffered health tech solutions which are out there.

What I couldn't understand is that **every single** current health tech solution is **database-backed**, and thereby inherently organisation-centric.

This includes solutions such as FHIR and OpenEHR, are designed to improve interoperability, however because they are still centralised and organisation-centric, database-backed solutions then they fall into the same trap as all the others.

It doesn't matter how large you make the organisations, eventually all organisations have their 'edges', and it is at the edges where you hit absolute and unresolvable problems of interoperability.

I've been puzzling this over for a decade, wondering if there can be a solution for this, and all the time learning more about how the tech world works, and what existing solutions can be brought into health from the wider tech world.

I've been using Git as a DVCS for around ten years as well, and it took me a long time for the penny to drop that what were experiencing in healthcare is the identical parallel of the CVS vs DVCS debate of 15-20 years ago in 'normal' tech. A debate that was unequivocally won by DVCS.

Right at the beginning of my health tech journey, I remember googling 'medical file format' because I thought maybe the solution was in this area. I didn't find much of use except some barmy XML dialect, and over time when I discussed files with technology people they were very disparaging about files, and pointed to all the work that was around databases. It's taken me all this time to learn about those systems and eventually come full circle right back to where I started.

**Files are the answer.**

In some ways it feels like starting completely from scratch again. In some ways it is. It doesn't mean we have to throw out everything that happened in the world of healthcare interoperability in the interim though. For example, we can learn a lot from FHIR and OpenEHR that will help to inform the structure of a health record.

!!! tip
    If it helps, you can do what my friend [Kevin Monk](https://twitter.com/kevinmonk) did and realised that a file is like a 'mini database all of its own', on a disk. And now relax.

## About Marcus Baw

I'm a GP in North Yorkshire, which is in the continent of Europe. I'm a proud Yorkshireman. I am a father, a guitarist, and a mountain biker although not necessarily in that order.

I qualified in Medicine from the University of Liverpool in 2000 and spent around 10 years in acute hospital specialities (Emergency Medicine, Anaesthesia and ICU) mostly in the Liverpool and Manchester region before deciding to change career paths and completing GP training in Wigan in 2011.

I'm a self taught software developer, so you are almost certainly better than me.

Somewhere between programming and clinical medicine is a nebulous area called Clinical Informatics. I was the Chair of the RCGP Health Informatics Group right through the COVID pandemic (2019-2022), and I'm a Fellow of the Faculty of Clinical Informatics.

twitter: @marcus_baw
github: pacharanero
